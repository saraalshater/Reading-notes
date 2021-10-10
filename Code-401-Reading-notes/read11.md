Spring App Basics
Spring MVC
What you need to build it:
Build an application that has a static home page and that will also accept HTTP GET requests at: http://localhost:8080/greeting
body of HTML that contains a greeting: “Hello, World!”
Customize the greeting with an optional name parameter in the query string, and the URL will look like this: http://localhost:8080/greeting?name=User
name parameter value overrides the default value of World and is reflected in the response by the content changing to “Hello, User!”
What you need: 15 minutes, text editor or IDE, JDK 1.8 or later, Gradle 4+, and import the code to IntelliJ or Spring Tool Suite.
How to complete this guide: start from scatch, clone this git clone https://github.com/spring-guides/gs-serving-web-content.git in to your terminal, cd into it, and create a web controller.
Spring initializr - use this to generate a new project with the required dependencies (Spring Web, Thymeleaf, and Spring Boot DevTools). If you use Gradle, visit the Spring Initializr to generate a new project with the required dependencies.
You can manually initialize it by navigating to https://start.spring.io, choose Gradle or Maven, click Dependencies and select Spring Web, Thymeleaf, and Spring Boot DevTools, and finally click generate. Download the resulting zip file.
Create a Web Controller:
HTTP requests are handled by a controller, and is identified by @Controller annotation.
GreetingController - handles GET requests for /greeting by returning the name of a View
View - is responsible for rendering the HTML content
@GetMapping annotation - ensures that HTTP GET requests to /greeting are mapped to the greeting() method
@RequestParam - binds the value of the query string parameter name into the name parameter of the greeting() method
Spring Boot Devtools - enables hot swapping, switches template engines to disable caching, enables LiveReload to automatically refresh the browser, and other reasonable defaults based on development instead of production.
Run the Application:
@SpringBootApplication - a convenient annotation that adds up:
@Configuration - tags the class as a source of bean definitions for the application context.
@EnableAutoConfiguration - tells Spring Boot to start adding beans based on classpath settings, other beans, and various property settings.
@ComponentScan - tells Spring to look for other components, configurations, and services in the com/example package, letting it find the controllers.
main() method - uses Spring Boot’s SpringApplication.run() method to launch an application
Build an executable JAR that contains all the necessary dependencies, classes, and resources and run that.
Test the app on http://localhost:8080/greeting, and provide a name query string parameter by visiting http://localhost:8080/greeting?name=User to see if the greeting changes or not.
Spring model attributes: (Links to an external site.)

Spring MVC calls the pieces of data that can be accessed during the execution of views model attributes. The equivalent term in Thymeleaf language is context variables.

There are several ways of adding model attributes to a view in Spring MVC. Below you will find some common cases:

Add attribute to Model via its addAttribute method:

  @RequestMapping(value = "message", method = RequestMethod.GET)
      public String messages(Model model) {
          model.addAttribute("messages", messageRepository.findAll());
          return "message/list";
      }


Return ModelAndView with model attributes included:

 @RequestMapping(value = "message", method = RequestMethod.GET)
      public ModelAndView messages() {
          ModelAndView mav = new ModelAndView("message/list");
          mav.addObject("messages", messageRepository.findAll());
          return mav;
      }


Expose common attributes via methods annotated with @ModelAttribute:

    @ModelAttribute("messages")
      public List<Message> messages() {
          return messageRepository.findAll();
      }