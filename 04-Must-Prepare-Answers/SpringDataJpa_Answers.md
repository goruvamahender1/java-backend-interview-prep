 ## SpringData Jpa Answers

---
 
#### 13.
 🔷 Java Persistence API (JPA)
1. JPA is a specification for managing relational data in Java apps.
2. Comes under jakarta.persistence package.
3. Provides standard APIs for ORM but doesn’t include actual implementation.
4. Uses EntityManagerFactory to interact with the persistence unit.
5. Uses EntityManager to perform CRUD operations & manage entities.
6. Uses JPQL (Java Persistence Query Language) for querying entities.
JpaRepository vs CrudRepository

🔶 Hibernate
1. Hibernate is a framework (ORM tool) that implements JPA specification.
2. Comes under org.hibernate package.
3.  Provides the implementation of JPA and adds extra features.
4. Uses SessionFactory to create Session instances.
5. Uses Session for CRUD operations – bridges the app and DB.
6. Uses HQL (Hibernate Query Language) for querying entities.