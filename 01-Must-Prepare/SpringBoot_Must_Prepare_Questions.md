## SpringBoot Must Prepare Questions

---

1. What are the main features of Spring Boot?  
2. How do you create a Spring Boot application?  
3. What is the difference between @Component, @Service, and @Repository?  
4. How does dependency injection work in Spring?  
5. What is Spring Boot Starter and how does it help?  
6. How does Spring Boot auto-configuration work?  
7. How do you configure properties in Spring Boot?  
8. How do you run different configurations for dev, test, and prod environments?  
9. What are @RestController and @Controller?  
10. How do you handle exceptions in Spring Boot?  
11. How do you customize error responses in REST APIs?  
12. What is REST and what are its key principles?  
13. What is the difference between PUT and POST?  
14. What are common pitfalls in REST API design?  
15. How do you ensure API backward compatibility?  
16. What is Spring Boot Actuator and how do you use it?  
17. How do you monitor health and metrics of a Spring Boot application?  
18. How do you manage secrets (e.g., DB credentials) in Spring Boot apps?  
19. What is the difference between constructor injection and field injection?  
20. What is caching? How have you used it in your applications?  
21. What is Spring Boot and how is it different from Spring Framework?  
22. What is the purpose of @RestController and how is it different from @Controller?  
23. What are the common annotations used in Spring Boot?  
24. What is dependency injection and how does Spring implement it?  
25. What is the use of @Autowired?  
26. How do you connect a Spring Boot app to a database?  
27. What is application.properties or application.yml used for?  
28. How do you create REST APIs using Spring Boot?  
29. How do you test REST APIs in Spring Boot?  
30. What is the folder structure of a Spring Boot project?  
31. What is REST? What are common HTTP methods used?
32. How do you create a project using Spring Initializr?
33. How do you connect a Spring Boot app to MySQL?
34. How do you call an external REST API in Java?
35. What is a repository interface in Spring?
36. How do you insert a document in MongoDB using Spring Data?
37. How do you log in Spring Boot?
38. What is a DTO?
39. What is @PathVariable vs @RequestParam?
40. How to return a list of objects from an API?
41. How to create scheduled tasks?
42. How to test an endpoint using Postman or curl?
43. How to create a custom response entity?
44. How to expose a REST API?
45. What is the purpose of @SpringBootApplication?
46. How do you read values from application.properties?
47. What do you understand by springboot in general?
48. Mention the benefits and limitations of Spring AOP?
49. What are the advantages of using Spring Boot? 
50. What are the Spring Boot key components? 
51. How does Spring Boot works? 
52. What does the @SpringBootApplication annotation do internally? 
53. What is the purpose of using @ComponentScan in the class files?
54. How does a Spring Boot application get started?
55. What is Spring Initializer?
56. What is Spring Boot CLI and what are its benefits?
57. What are the most common Spring Boot CLI commands?
58. What Are the Basic Annotations that Spring Boot Offers?
59. What is Spring Boot dependency management?
60. Can we create a non-web application in Spring Boot? 
61. Is it possible to change the port of the embedded Tomcat server in Spring Boot?
62. What is the default port of Tomcat in Spring Boot?
63. Can we override or replace the Embedded Tomcat server in Spring Boot?
64. Can we disable the default web server in the Spring Boot application?
65. How to disable a specific auto-configuration class?
66. Difference b/w @RequestMapping, @GetMapping, @PostMapping, @PutMapping, @DeleteMapping, @PatchMapping
67. Describe the flow of HTTPS requests through the Spring Boot application?
68. What is the use of Profiles in Spring Boot?
69. How to enable Actuator in Spring Boot application? 
70. What are the actuator-provided endpoints used for monitoring the Spring Boot application? 
71. How to get the list of all the beans in your Spring Boot application?
72. How to check the environment properties in your Spring Boot application? 
73. What is vault?
74. How to enable debugging log in the Spring Boot application?
75. Where do we define properties in the Spring Boot application?   
76. What is an IOC container?
77. Explain Spring Boot's run() Method?
78. Explain Validations in Spring Boot i.e., @Valid, @NotNull, @Size, and create custom validation annotations.
79. Explain Relaxed Binding in Spring Boot i.e., Learn how Spring Boot auto-binds configuration properties, making externalized configuration flexible and powerful.
80. Properties vs YAML – Should you use .properties or .yaml for configuration? Understand the differences and best practices?
81. What is @Profile and how the Manage multiple environments using it?
82. Difference b/w @Qualifier vs @Primary and when this are being used?
83. What Are DispatcherServlet and ContextLoaderListener?
84. Difference between BeanFactory and application context?
85. What are Spring MVC interceptors?
86. Can you create a controller without using @Controller or @RestController annotations?
87. How is the root application context in Spring MVC loaded?
88. Name the exceptions thrown by the Spring DAO classes.
89. Explain Spring bean lifecycle ?
90. How to implement Custom validator other than predefined?
91. What are some common performance tuning practices in a Spring Boot application?
92. How would you implement asynchronous processing in Spring Boot?
93. How do you handle Gateway Timeout (504) and Service Unavailable (503) errors in a project?
94. What is the ApplicationContext in Spring?
95. What are the advantages of using Spring Boot?
96. What are the different scopes available in Spring?
97. What is @Mockito and how is it used in testing?
98. What is the difference between prototype and request scope in Spring?
99. How do you handle Dependency Injection in Spring Boot?
100. What are the commonly used HTTP error codes in applications?
101. What do 404, 402, 502, 503, and 401 HTTP error codes mean?
102. What is the difference between @Bean and @Autowired in Spring?
103. How do you handle a "Not Found" (404) error in Spring Boot?
104. What typically causes a "Bad Request" (400) error?
105. Are the server port and debug port the same in a Spring Boot application?
106. When should you use and when should you avoid using @Mock?
107. How do you handle "Service Not Found" errors even when beans are properly registered?
108. How do you debug issues in both local and remote repositories?
109. What are Helper classes, Utility classes, and Data Transfer Objects (DTOs) in Java?
110. A user triggers a long-running operation (e.g., report generation). How would you ensure a non-blocking experience?Use @Async with @EnableAsync Return a CompletableFuture<> or use messaging queues like RabbitMQ or Kafka
Notify the user via WebSocket, polling, or email
111. What is the difference between a DTO class and a record class in Java?
112. What architecture are you using in your Spring Boot application?
113. What are the core rules and best practices of REST API design?
114. If the Department is part of another microservice, how would you access its data?
115. What are the disadvantages of using Spring Boot?
116. PUT vs POST — interchangeable or not?
117. What happens if you swap @Service and @Repository?
118. HTTP 403 vs 404 — what do they mean?
119. How do you make a contact between two HTTPS? You want to send a request to another HTTPS and get the response ?
120. What is Junit and what are the methods available in Junit?
121. How does the @RestControllerAdvice annotation work in Spring Boot for global exception handling?
122. Explain the Builder design pattern. When is it preferable over telescoping constructors?
123. Query Params vs Path Variables
124. What is the difference between eager and lazy initialization in Java? How does Spring support both?
125. How does the @RequestScope, @SessionScope, and @ApplicationScope work in Spring?
126. What version of Spring and java did you use?
127.  Different types of request bodies in REST APIs?
128. What are module attributes in a project?
129. What are the types of bean scopes in Spring?
130. Explain the life cycle of a Spring Bean?
131. @WebMvcTest, @DataJpaTest, and Mockito for testing controllers and repositories.
132. Implement @ControllerAdvice and @ExceptionHandler for centralized error handling.
133. Can we have @SpringBootApplication classes in the same project.
134. How do you configure multiple data sources in Spring Boot?
135. How do you write parameterized tests in JUnit 5?
136. How do you externalize configuration using YAML and Properties files?
137. Feign Client vs WebClient: Which one to use and why.
138. What’s the difference between Filters and Interceptors?
139. Can we use @Component instead of @Repository?
140. Write the code for different injections constructor, field, setter injection and which is recommended and why.
141. How do you GET is more faster than POST?
142. What are the HTTP methods?
143. Differentiate the Status Code 400 series and 500 series
144. How do annotations like @Transactional work internally in Spring? What is proxy-based AOP?
145. How do you handle circular dependencies in Spring? What are common solutions or design alternatives?
146. Explain the role of transient and serialVersionUID in Java serialization.
147. How do @JsonIgnore, @JsonProperty, and @JsonInclude annotations work in Jackson? When and why would you use them in a Spring Boot application?
148.  What are the most commonly used Jackson annotations in Spring Boot for JSON serialization/deserialization, and how do they work? Explain with examples for:
```
@JsonIgnore
@JsonProperty
@JsonInclude
@JsonFormat
@JsonCreator
@JsonValue
@JsonAlias
@JsonAnyGetter / @JsonAnySetter
@JsonAutoDetect
@JsonDeserialize / @JsonSerialize
```