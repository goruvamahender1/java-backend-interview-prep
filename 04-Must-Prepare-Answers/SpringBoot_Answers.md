## SpringBoot Must Prepare Questions

---
#### 23.
✅ 1. Spring Boot Core Annotations
| Annotation                 | Purpose                                                                                                                 |
| -------------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| `@SpringBootApplication`   | Marks the main class of a Spring Boot app (combines `@Configuration`, `@EnableAutoConfiguration`, and `@ComponentScan`) |
| `@EnableAutoConfiguration` | Enables Spring Boot’s auto-configuration                                                                                |
| `@ComponentScan`           | Scans packages for components to register as beans                                                                      |
| `@Configuration`           | Indicates a class contains bean definitions                                                                             |

✅ 2. Component Annotations (Stereotypes)
| Annotation        | Purpose                                                          |
| ----------------- | ---------------------------------------------------------------- |
| `@Component`      | Generic component class (detected during component scanning)     |
| `@Service`        | Specialization of `@Component`, used for service layer classes   |
| `@Repository`     | DAO layer; enables exception translation                         |
| `@Controller`     | MVC controller (typically returns views)                         |
| `@RestController` | Combination of `@Controller` + `@ResponseBody`, returns JSON/XML |

✅ 3. Dependency Injection
| Annotation   | Purpose                                                               |
| ------------ | --------------------------------------------------------------------- |
| `@Autowired` | Injects a bean automatically by type                                  |
| `@Qualifier` | Disambiguates injection when multiple beans of the same type exist    |
| `@Value`     | Injects values from `application.properties` or environment variables |
| `@Bean`      | Declares a bean explicitly inside a `@Configuration` class            |

✅ 4. Web / REST Mapping Annotations
| Annotation        | HTTP Method                                     |
| ----------------- | ----------------------------------------------- |
| `@RequestMapping` | Generic mapping for any HTTP method             |
| `@GetMapping`     | Handles GET requests                            |
| `@PostMapping`    | Handles POST requests                           |
| `@PutMapping`     | Handles PUT requests                            |
| `@DeleteMapping`  | Handles DELETE requests                         |
| `@PatchMapping`   | Handles PATCH requests                          |
| `@PathVariable`   | Binds URL template variable to method parameter |
| `@RequestParam`   | Extracts query parameters                       |
| `@RequestBody`    | Binds request body to a method parameter        |
| `@ResponseBody`   | Returns Java object as response (usually JSON)  |
| `@ResponseStatus` | Sets HTTP status code for a method              |

✅ 5. Validation
| Annotation                          | Purpose                                        |
| ----------------------------------- | ---------------------------------------------- |
| `@Valid` / `@Validated`             | Triggers validation before method executes     |
| `@NotNull`, `@Size`, `@Email`, etc. | Bean validation constraints (javax or jakarta) |

✅ 6. Spring Boot Testing
| Annotation        | Purpose                                              |
| ----------------- | ---------------------------------------------------- |
| `@SpringBootTest` | Loads full application context for integration tests |
| `@WebMvcTest`     | Loads only web layer components                      |
| `@MockBean`       | Adds a mocked bean to Spring context                 |
| `@DataJpaTest`    | Configures in-memory DB and tests JPA repositories   |

✅ 7. Spring Data JPA
| Annotation                                             | Purpose                                   |
| ------------------------------------------------------ | ----------------------------------------- |
| `@Entity`                                              | Marks a class as a JPA entity             |
| `@Table`                                               | Customizes table name for entity          |
| `@Id`                                                  | Specifies primary key                     |
| `@GeneratedValue`                                      | Auto-generates primary key                |
| `@OneToMany`, `@ManyToOne`, `@OneToOne`, `@ManyToMany` | Define relationships                      |
| `@Repository`                                          | Marks interface as Spring Data repository |
| `@Query`                                               | Write custom JPQL/SQL queries             |
