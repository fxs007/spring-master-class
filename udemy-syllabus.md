Syllabus of udemy spring-tutorial-for-beginners
# 01-spring-in-depth
- Step 1 - Setting up a Spring Project using htttp://start.spring.io
- Step 2 - Understanding Tight Coupling using the Binary Search Algorithm Example
- Step 3 - Making the Binary Search Algorithm Example Loosely Coupled
- Step 4 - Using Spring to Manage Dependencies - @Component, @Autowired
- Step 5 - What is happening in the background?
- Step 6 - Dynamic auto wiring and Troubleshooting - @Primary
- Step 7 - Constructor and Setter Injection
- Step 8 - Spring Modules
- Step 9 - Spring Projects
- Step 10 - Why is Spring Popular?
- Step 11 - Dependency Injection - A few more examples
- Step 12 - Autowiring in Depth - by Name and @Primary
- Step 13 - Autowiring in Depth - @Qualifier annotation
- Step 14 - Scope of a Bean - Prototype and Singleton
- Step 15 - Complex scenarios with Scope of a Spring Bean - Mix of Prototype and Singleton
- Step 15B -  Difference Between Spring Singleton and GOF Singleton
- Step 16 - Using Component Scan to scan for beans
- Step 17 - Lifecycle of a Bean - @PostConstruct and @PreDestroy
- Step 18 - Container and Dependency Injection (CDI) - @Named, @Inject
- Step 19 - **Removing Spring Boot in Basic Application**
- Step 20 - Fixing minor stuff - Add Logback and Close Application Context
- Step 21 - Defining Spring Application Context using XML - Part 1
- Step 22 - Defining Spring Application Context using XML - Part 2
- Step 23 - Mixing XML Context with Component Scan for Beans defined with Annotations
- Step 24 - IOC Container vs Application Context vs Bean Factory
- Step 25 - @Component vs @Service vs @Repository vs @Controller
- Step 26 - **Read values from external properties file**

## Use diff

- diff Step18.md Step19.md
- diff Step18.md Step19.md --side-by-side --width=200 | less

# 00-framework-tool-introductions/03.JUnit-Introduction-In-5-Steps

# 00-framework-tool-introductions/04.Mockito-Introduction-In-5-Steps
- @Mock
- @InjectMocks.
- @RunWith

# unit test with Spring : 01-spring-in-depth
- Step 27 - Spring Unit Testing with a Java Context
- Step 28 - Spring Unit Testing with an XML Context
- Step 29 - Spring Unit Testing with Mockito

- @Mock creates a mock. @InjectMocks creates an instance of the classand injects the mocks that are created with the @Mock (or @Spy). You must use @Runwith(MockitoJUnitRunner.class) or Mockito.initMocks(this) to initialize these mocks and inject them.
```java
@RunWith(MockitoJUnitRunner.class)
public class SomeCdiBusinessTest {
    //Inject Mock
    @InjectMocks
    SomeCdiBusiness business;

    //Create Mock
    @Mock
    SomeCdiDao daoMock;

    @Test
    public void testBasicScenario() {
        //when daoMock.getData() method is called, return int[] {2,4}
        Mockito.when(daoMock.getData()).thenReturn(new int[] {2,4});
        int actualResult = business.findGreatest();
        assertEquals(4, actualResult);
    }
}
```
- Suggest to choose Mockito over Spring unit test. But sometimes (e.g. Spring MVC), you have to use Spring unit test.

# 00-framework-tool-introductions/01.Eclipse-Introduction-in-5-steps

# 00-framework-tool-introductions/05.Spring-Boot-Introduction-In-10-Steps

# 04-spring-jdbc-to-jpa
- http://www.in28minutes.com/jpa-hibernate-tutorial-for-beginners

# 02-basic-web-application


