# Hibernate, JPA, and JDBC Cheat Sheet

## JDBC (Java Database Connectivity)

### Core Classes and Utilities

- `JdbcTemplate`: Core class in Spring JDBC that simplifies the use of JDBC and helps manage resources.
- `NamedParameterJdbcTemplate`: Extension of `JdbcTemplate` that allows parameters to be named instead of indexed.
- `SimpleJdbcInsert`: Class to simplify the process of inserting data into a database table using JDBC.
- `SimpleJdbcCall`: Class to simplify the process of executing stored procedures or functions using JDBC.
- Exception Handling: Strategies for handling exceptions and errors in JDBC operations, such as `DataAccessException`.
- RowMapper Interface: Interface for mapping rows of a `ResultSet` to domain objects.
- `DriverManager`: Utility class for managing a set of JDBC drivers.

## JPA (Java Persistence API)

### Annotations

- `@Entity`: Specifies that a class is an entity.
- `@Table`: Specifies the table name for an entity.
- `@Id`: Specifies the primary key of an entity.
- `@GeneratedValue`: Specifies automatic generation of primary key values.
- `@OneToOne`, `@OneToMany`, `@ManyToOne`, `@ManyToMany`: Annotations to define different types of entity relationships.
- `@Repository`: Annotation indicating that a class is a repository, typically for database access.
- `@EntityScan`: Annotation to specify the base packages for entity scanning.
- `@EnableJpaRepositories`: Annotation to enable JPA repositories in the Spring application context.
- `@Query`: Annotation to define custom JPQL, SQL, or native queries directly in repository interfaces.
- `@Transactional`: Annotation to declare transactional methods or classes.

### Interfaces and Classes

- `javax.persistence.EntityManager`: Interface representing an entity manager, which interacts with the persistence context.
- `javax.persistence.Query`: Interface representing a query object for executing JPQL (Java Persistence Query Language) queries.
- `JpaRepository`: Interface providing CRUD operations and additional methods for working with entities.

### Utilities

- `javax.persistence.Persistence`: Utility class for obtaining a persistence unit, which manages entity managers.
- Spring Data Query Methods: Convention-based query creation by defining method names in repository interfaces.
- Spring Data Pagination: Support for paginated queries using `Pageable` and `Page` interfaces.

## Hibernate

### Core Concepts

- Hibernate Session: Represents a single-threaded unit of work for interacting with the database.
- Hibernate SessionFactory: Represents a factory for Hibernate sessions.
- Hibernate Criteria API: Programmatic way of creating queries in Hibernate using a fluent interface.
- Hibernate HQL (Hibernate Query Language): Hibernate-specific query language similar to SQL but operates on entities.
- Hibernate Native SQL: Direct use of SQL queries with Hibernate.
- Hibernate Caching: Mechanism to store frequently accessed data in memory for faster access.
- Hibernate Transaction: Unit of work performed against a database.
- Hibernate Cascade Types: Defines how entity state transitions (e.g., save, update, delete) propagate to associated entities.

## Reference

- [Hibernate Documentation](https://hibernate.org/orm/documentation/5.5/)
- [Spring Data JPA Documentation](https://docs.spring.io/spring-data/jpa/docs/current/reference/html/)
- [Spring JDBC Documentation](https://docs.spring.io/spring-framework/docs/current/reference/html/data-access.html#jdbc)
