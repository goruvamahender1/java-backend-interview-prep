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

#### 115. 
🔍 Disadvantages of Spring Boot (Worth Considering):
- ⚙️ **Auto-Configuration is a Black Box**  
  While convenient, it hides internal behaviors — harder to debug or customize deeply.

- 🐘 **Higher Memory & Startup Time**  
  Not ideal for low-memory or fast-boot scenarios (like serverless).

- 📦 **Fat JAR Size**  
  Spring Boot apps tend to package all dependencies, leading to large artifacts (~50–100MB+).

- 🧰 **Overkill for Simple Tools**  
  For lightweight tasks or utilities, it may add unnecessary complexity.

- 🧩 **Tuning Can Be Tricky**  
  Multiple abstraction layers make performance tuning and profiling less straightforward.

- 🔗 **Tight Coupling with Spring Ecosystem**  
  Once you adopt Spring Boot, switching away isn’t easy.

- 📚 **Advanced Customization Requires Deep Knowledge**  
  Disabling or altering default behaviors (like auto-config) demands in-depth Spring experience.

- ✅ **Spring Boot is fantastic for enterprise applications, but it’s not one-size-fits-all.**  
  🎯 Being aware of its trade-offs helps us make better architectural decisions — especially as Technical Leads or Architects.

#### 134. 
Yes, you can have multiple @SpringBootApplication classes — especially in modular applications or when writing tests — but only one should be used to bootstrap the application.

💡 Example Use Case
Imagine you’re building an app with separate modules for UserService and AdminService. Each module can have its own main() class for testing or running separately.
```
// src/main/java/com/example/user/UserApplication.java
@SpringBootApplication
public class UserApplication {
 public static void main(String[] args) {
 SpringApplication.run(UserApplication.class, args);
 }
}
```
```
// src/main/java/com/example/admin/AdminApplication.java
@SpringBootApplication
public class AdminApplication {
 public static void main(String[] args) {
 SpringApplication.run(AdminApplication.class, args);
 }
}
```

🔄 Important Note: When deploying or building the final app, make sure only one of these classes is used to start the application, or you may run into conflicts