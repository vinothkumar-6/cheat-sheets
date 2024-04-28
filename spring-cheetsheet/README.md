# Spring Basics Cheat Sheet


## Dependency Injection

| Concept                  | Description                                                                                                   |
| ------------------------ | ------------------------------------------------------------------------------------------------------------- |
| `@Autowired`             | Annotation used to automatically wire beans by type.                                                          |
| `@Qualifier`             | Annotation used to specify which bean to autowire when multiple beans of the same type are present.           |
| `@Component`             | Annotation used to mark a Java class as a Spring component.                                                  |
| `@Repository`            | Annotation used to indicate that a class is a repository.                                                     |
| `@Service`               | Annotation used to indicate that a class is a service.                                                        |
| `@Controller`            | Annotation used to mark a class as a Spring MVC controller.                                                   |

## Spring Boot

| Concept                  | Description                                                                                                   |
| ------------------------ | ------------------------------------------------------------------------------------------------------------- |
| `@SpringBootApplication`| Annotation used to enable Spring Boot features in an application.                                             |
| `@EnableAutoConfiguration`| Annotation used to enable Spring Boot's auto-configuration mechanism.                                       |
| `@Configuration`         | Annotation used to specify that a class declares one or more bean definitions.                                |
| `@RestController`        | Annotation used to combine `@Controller` and `@ResponseBody`, indicating that the return value should be serialized directly into the HTTP response body.|

## Spring MVC

| Concept                  | Description                                                                                                   |
| ------------------------ | ------------------------------------------------------------------------------------------------------------- |
| `@RequestMapping`        | Annotation used to map web requests to specific handler methods.                                              |
| `@PathVariable`          | Annotation used to extract values from the URI template.                                                       |
| `@RequestParam`          | Annotation used to extract query parameters from the request URL.                                              |
| `@ModelAttribute`        | Annotation used to bind request parameters to model attributes.                                               |
| `@ResponseBody`          | Annotation used to indicate that a method return value should be bound to the web response body.              |
| `ModelAndView`           | Class representing both the model and the view in a Spring MVC application.                                    |
| `ViewResolver`           | Interface for classes that resolve view names to actual view objects.                                          |
| `RedirectView`           | Class representing a view that redirects to another URL.                                                       |

## Spring Data JPA

| Concept                  | Description                                                                                                   |
| ------------------------ | ------------------------------------------------------------------------------------------------------------- |
| `@Entity`                | Annotation used to define a JPA entity class.                                                                 |
| `@Repository`            | Annotation used to indicate that a class is a repository.                                                     |
| `@Transactional`         | Annotation used to mark a method as transactional.                                                             |
| `CrudRepository`         | Interface providing CRUD operations for a specific entity.                                                     |
| `JpaRepository`          | Interface extending `CrudRepository` with additional JPA-specific methods.                                     |

## Spring Security

| Concept                  | Description                                                                                                   |
| ------------------------ | ------------------------------------------------------------------------------------------------------------- |
| `@EnableWebSecurity`     | Annotation used to enable Spring Security's web security support.                                              |
| `WebSecurityConfigurerAdapter` | Class providing default security configurations for web applications.                                        |
| `@Secured`               | Annotation used to specify that a method requires certain security constraints to be fulfilled.              |
| `@PreAuthorize`          | Annotation used to specify that a method should be allowed to proceed only if the specified condition is met. |

## Spring Bean Scopes

| Concept                  | Description                                                                                                   |
| ------------------------ | ------------------------------------------------------------------------------------------------------------- |
| `singleton`              | Scope indicating that a single instance of the bean is created for each Spring IoC container.                |
| `prototype`              | Scope indicating that a new instance of the bean is created each time it is requested.                        |
| `request`                | Scope indicating that a new instance of the bean is created for each HTTP request.                            |
| `session`                | Scope indicating that a new instance of the bean is created for each HTTP session.                            |
| `application`            | Scope indicating that a single instance of the bean is created for the lifetime of the application context.   |

## Spring AOP

| Concept                  | Description                                                                                                   |
| ------------------------ | ------------------------------------------------------------------------------------------------------------- |
| `@Aspect`                | Annotation used to mark a class as an aspect.                                                                 |
| `@Pointcut`              | Annotation used to define a pointcut, which is a predicate that matches method executions.                    |
| `@Before`                | Annotation used to indicate that advice should run before the matched method execution.                       |
| `@AfterReturning`        | Annotation used to indicate that advice should run after a matched method returns successfully.               |
| `@AfterThrowing`         | Annotation used to indicate that advice should run after a matched method throws an exception.                |
| `@Around`                | Annotation used to indicate that advice should run around a matched method execution.                         |

## Spring Testing

| Concept                  | Description                                                                                                   |
| ------------------------ | ------------------------------------------------------------------------------------------------------------- |
| `@SpringBootTest`        | Annotation used to create a Spring ApplicationContext for integration tests.                                  |
| `@WebMvcTest`            | Annotation used to configure Spring MVC tests.                                                                |
| `@DataJpaTest`           | Annotation used to configure tests that are JPA specific.                                                      |
| `@MockBean`              | Annotation used to mock a bean in a Spring application context.                                                |
| `@Test`                  | Annotation used to mark a method as a test method.                                                            |
| `@Before`                | Annotation used to indicate that a method should be run before each test method.                               |
| `@After`                 | Annotation used to indicate that a method should be run after each test method.                                |
| `@RunWith`               | Annotation used to specify a custom test runner.                                                               |

## Spring Boot Actuator

| Concept                  | Description                                                                                                   |
| ------------------------ | ------------------------------------------------------------------------------------------------------------- |
| `/actuator`              | Endpoint providing operational information about the application.                                              |
| `/health`                | Endpoint providing information about the health of the application.                                             |
| `/info`                  | Endpoint providing arbitrary application information.                                                          |
| `/metrics`               | Endpoint providing information about application metrics.                                                       |
| `/env`                   | Endpoint providing information about the application's environment.                                              |
| `/beans`                 | Endpoint providing information about the application's beans.                                                    |

## Reference

- [Spring Documentation](https://spring.io/docs)
