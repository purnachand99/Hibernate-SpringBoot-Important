**[How To Use JPA Named Queries Via Annotations](https://github.com/AnghelLeonard/Hibernate-SpringBoot/tree/master/HibernateSpringBootNamedQueriesViaAnnotations)**
  
**Description:** JPA named (native) queries are commonly written via `@NamedQuery` and `@NamedNativeQuery` annotations in entity classes.  This application shows you how to do it. But, keep in mind that dynamic sorting (`Sort`) and pagination via `Pageable` doesn't work at full capacity in this approach. More precisely, `Sort` will be ignored and `Pageable` will ask you to provide the `SELECT COUNT` via `countQuery`. At least this is how it behave in Spring Boot 2.2.2.

The best approach that supports dynamic sorting, pagination and slicing relies on using a [properties](https://github.com/AnghelLeonard/Hibernate-SpringBoot/tree/master/HibernateSpringBootNamedQueriesInPropertiesFile) file for listing the named (native) queries.
 
**Key points:**
- use `@NamedQuery` and `@NamedNativeQuery` annotations in entity classes
- follow the Spring `{EntityName}.{RepositoryMethodName}` naming convention for a quick and slim implementation
- avoid `Sort` and `Pageable`

-----------------------------------------------------------------------------------------------------------------------    
<table>
     <tr><td><b>If you need a deep dive into the performance recipes exposed in this repository then I am sure that you will love my book "Spring Boot Persistence Best Practices"</b></td><td><b>If you need a hand of tips and illustrations of 100+ Java persistence performance issues then "Java Persistence Performance Illustrated Guide" is for you.</b></td></tr>
     <tr><td>
<a href="https://www.apress.com/us/book/9781484256251"><p align="left"><img src="https://github.com/AnghelLeonard/Hibernate-SpringBoot/blob/master/Spring%20Boot%20Persistence%20Best%20Practices.jpg" height="500" width="450"/></p></a>
</td><td>
<a href="https://leanpub.com/java-persistence-performance-illustrated-guide"><p align="right"><img src="https://github.com/AnghelLeonard/Hibernate-SpringBoot/blob/master/Java%20Persistence%20Performance%20Illustrated%20Guide.jpg" height="500" width="450"/></p></a>
</td></tr></table>

-----------------------------------------------------------------------------------------------------------------------    
