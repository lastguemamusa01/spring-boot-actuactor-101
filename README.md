# spring-boot-actuactor-101


Web services – http service. Interoperability. A2A  Application to Application. Not platform dependent.

Library – create jar for backend and database. Locally. Not updated automatically. 
Rest services – spring boot, JPA
Microservices – spring cloud


Service definition – endpoint, format(xml, json), request and response structure, Transport(http or mq – message queue)
Soap(Simple object access protocol) – restriction approach only xml
-	Envelop, Header(meta-data like authtenticantion, authorization and signature, etc) and body(real content)
-	Service definition – WSDL(Web service definition language)(mandatory) – endpoints, all operations, request and response structure
-	Can be Message queue or HTTP
Rest(Represental state tranfer) – architecture approach and only http , no restriction of the use of representation(xml, json(prefered))
-	Service definition – WADL(Web application definition language) or swagger(popular). – headers, body, method(get, pot), status code(404), 
-	All is resource(abstraction) and resource is what will be exposed to outside(the world) using URI(/user/Ranga/todos/1)

Rest api is more easy than soap.

Spring boot – enable building production ready applications quickly, providing embedded servers(tomcat, jetty), metrics, health checks and externalized configuration.

Starter projects with auto configuration – spring mvc, spring core, jpa(hibernate)
Spring boot actuactor – monitoring your application
Support environment(dev, vnv and prod)

Before spring boot, we need to add all framework to use like spring mvc, security ,etc. implement default exceptionController handling, create spring configuration file, configure resolver, configure web.xml – configure dispatcher server, internationalization, logging, etc. (spring boot starter web with spring boot stater security)

Spring boot – focus on business logic, todo lo anterior ya esta implementado en spring boot.

Autoconfiguration  - dispatcher and resolver configured automatically
Annotation - @SpringBootApplication -> this is spring context file, enable auto configuration, enable component scan(scan classes of the package for any beans). See for annotation.

Spring vs spring mvc vs spring boot
Own roles
Spring – testability – dependency injection – core of spring framework – IOC – inversion of control – help build loosely coupled applications that can be easily unit tested.  @Autowired to inject service in the controller

JDBC use try catch exception boilder code
Hibernate for ORM
Junit & Mockito for Unit testing

Spring MVC – concerned with developing web applications. Dispatcher Servlet, ModelAndView,View Resolver. Sepration of concerns

Pom.xml
Spring boot starter web – for web applications and rest api services
Spring boot starter test – junit, mockit
Spring boot starter data jpa – interface for hibernate
Those create maven dependencies


Spring-boot-starter-web-services – soap web services
Spring boot starter web – web and restful applications
Spring boot starter :
	Test – unit and integration testing
	Jdbc – traditional JDBC
	Hateoas – add hateoas feature to your restful services
	Security – authentication and authorization (basic, oauth and oauth2)
	Data-jpa – jpa(user default hibernate as the ORM framework) 
	Cache – enabling spring frameworks caching support(distributing caches like hazelcast)
	Data-rest – expose(jpa entities) simple rest services using spring data rest
	Actuator – advanced features like monitoring and tracing to your app
	Undertow, jetty, tomcat – choose your embedded servlet container
Logging – for logging using logback
	Log4j2 – logging using log4j2

With actuactor your can read a lot of metadata about the application
Hal standard – hal browser

Loaded automatically change – 

<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-devtools</artifactId>
</dependency>

