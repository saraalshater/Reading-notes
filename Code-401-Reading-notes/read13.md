## Working with Relationships in Spring Data REST
###  how to work with relationships between entities in Spring Data REST?

#### One-to-One Relationship

##### 1.  The Data Model

you can do two entity classes Library and Address having a one-to-one relationship using `@OneToOne`

@RestResource is optional 

We must be careful to have different names for each association resource. Otherwise, we will encounter a JsonMappingException with the message: “Detected multiple association links with same relation type! Disambiguate association”.


##### 2 . The Repositories
In order to expose these entities as resources, let's create two repository interfaces for each of them, by extending the `CrudRepository` interface:


`public interface LibraryRepository extends CrudRepository<Library, Long> {}` 
`public interface AddressRepository extends CrudRepository<Address, Long> {}`


##### 2.3. Creating the Resources



## One-to-Many Relationship
A one-to-many relationship is defined using the @OneToMany and @ManyToOne annotations and can have the optional @RestResource annotation to customize the association resource.


##  Many-to-Many Relationship
A many-to-many relationship is defined using @ManyToMany annotation, to which we can add @RestResource.

---------------------------------------------

# Integration Testing in Spring

Integration testing plays an important role in the application development cycle by verifying the end-to-end behavior of a system.

## Spring MVC Test Configuration


## Enable Spring in Tests with JUnit 5
Unit 5 defines an extension interface through which classes can integrate with the JUnit test.

We can enable this extension by adding the `@ExtendWith` annotation to our test classes and specifying the extension class to load. **To run the Spring test, we use SpringExtension.class.**

We also need the **@ContextConfiguration** annotation to load the context configuration and bootstrap the context that our test will use.

## The WebApplicationContext Object
WebApplicationContext provides a web application configuration. It loads all the application beans and controllers into the context.

## Mocking Web Context Beans
MockMvc provides support for Spring MVC testing. It encapsulates all web application beans and makes them available for testing.

## Verify Test Configuration




