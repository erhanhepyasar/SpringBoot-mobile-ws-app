Project: User Login, Spring Boot Application

Technologies and techniques used in the project
--------------------------------------------------
- Spring Boot dependencies:
	- Web starter
	- Spring Data JPA
	- Security
	- MySql JDBC Drive	
	- Lombok (Used for getters/setters, default constructor, toString, hashCode and equals)
- Spring Security: 
	- Web service endpoints are protected (Response: Status: 401 Unauthorized)
	- Encrypt user password with BCryptPasswordEncoder from SF before storing into db	
- Pom.xml: 
	- Spring Boot dependencies (listed above). Dependency versions are managed by spring boot.
	- Json web token (Added from Maven repository): For generating tokens
- Layered architecture:
	- Entity 
	- Service 
	- Controller: Rest CRUD operation mappings with annotations
	- Shared: DTO, Utils
	- DTO (Data Transfer Object) and BeanUtils.copyProperties() method to transfer objects between layers
- Utils:
	- Random String generator to generate userId and ...
- MySQL Server: Database and users were created manually. Tables are being created by Hibernate during application launch



Source: Udemy, RESTful Web Services, Java, Spring Boot, Spring MVC and JPA
