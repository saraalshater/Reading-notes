# [Spring Security Architecture](https://spring.io/guides/topicals/spring-security-architecture/)

## Authentication and Access Control

**Authentication** (who are you?)

**Authorization or Access control** (what are you allwoed to do ?)

## Authentication 

interface for authentication is `AuthenticationManager`
```

    public interface AuthenticationManager {

  Authentication authenticate(Authentication authentication)
    throws AuthenticationException;
}

```

`AuthenticationManager` can do three things in it is `authenticate()` method:
 - Return an Authentication (normally with authenticated=true) if it can verify that the input represents a valid principal.

 - Throw an AuthenticationException if it believes that the input represents an invalid principal.
 - Return null if it cannot decide.


`AuthenticationProvider` is a bit like an `AuthenticationManager`, but it has an extra method to allow the caller to query whether it supports a given `Authentication` type:


```
public interface AuthenticationProvider {

	Authentication authenticate(Authentication authentication)
			throws AuthenticationException;

	boolean supports(Class<?> authentication);
}
```


## Customizing Authentication Managers

Spring Security provides some **configuration helpers** to quickly get common authentication manager features set up in your application. The most commonly used helper is the `AuthenticationManagerBuilder`, which is great for setting up **in-memory**.


the `AuthenticationManagerBuilder` is `@Autowired` into a method in a `@Bean` — that is what makes it build the global (parent) `AuthenticationManager`.


```
@Configuration
public class ApplicationSecurity extends WebSecurityConfigurerAdapter {

  @Autowired
  DataSource dataSource;

   ... // web stuff here

  @Override
  public void configure(AuthenticationManagerBuilder builder) {
    builder.jdbcAuthentication().dataSource(dataSource).withUser("dave")
      .password("secret").roles("USER");
  }

}
```


If we had used an `@Override` of a method in the configurer, the `AuthenticationManagerBuilder` would be used only to build a **“local”** `AuthenticationManager`, which would be a **child of the global one**. In a Spring Boot application, you can `@Autowired` the global one into another bean, but you cannot do that with the local one unless you explicitly expose it yourself.


## Authorization or Access Control

The core strategy here is `AccessDecisionManager`. There are three implementations provided by the framework and all three delegate to a chain of `AccessDecisionVoter` instances.

An `AccessDecisionVoter` considers an `Authentication` (representing a principal) and a secure `Object`, which has been decorated with `ConfigAttributes`.



The `Object` is completely generic in the signatures of the `AccessDecisionManager` and `AccessDecisionVoter`. It represents anything that a user might want to access (a web resource or a method in a Java class are the two most common cases).

The `ConfigAttributes` are also fairly generic, representing a decoration of the secure `Object` with some metadata that determines the level of permission required to access it.


`ConfigAttribute` is an **interface**. It has only **one method** (which is quite generic and returns a `String`), so these strings encode in some way the intention of the owner of the resource, expressing rules about who is allowed to access it.

A typical `ConfigAttribute` is the name of a user role (like ROLE_ADMIN or ROLE_AUDIT), and they often have special formats (like the ROLE_ prefix) or represent expressions that need to be evaluated.

--------------------------------


## Web Security

Spring Security in the web tier (for UIs and HTTP back ends) is based on **Servlet Filters.**

The order of the filter chain is very important, and Spring Boot manages it through two mechanisms: `@Beans` of type Filter can have an` @Order` or implement Ordered, and they can be part of a `FilterRegistrationBean` that itself has an order as part of its API.

In a Spring Boot application, the security filter is a `@Bean` in the `ApplicationContext`, and it is installed by default so that it is applied to every request. 



# [Spring Auth Cheat Sheet](https://github.com/codefellows/seattle-java-401d2/blob/master/SpringAuthCheatSheet.md)


1.  set up a user model and repo
2. create a controller for that model
3. UserDetailsServiceImpl implements UserDetailsService
4.  ApplicationUser implements UserDetails : use IntelliJ to implement the methods; make the boolean ones all return true
5.  WebSecurityConfig extends WebSecurityConfigurerAdapter
 - has a UserDetailsService
 - passwordEncoder bean
 - configure AuthManagerBuilder
 `auth.userDetailsService(userDetailsService).passwordEncoder(passwordEncoder());`
 - configure HttpSecurity

6. registration page
 - create it w/ form
 - ensure it posts to a route your controller is ready for 
 - check it's saving in the DB


7. login page
