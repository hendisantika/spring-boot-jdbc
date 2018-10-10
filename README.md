# Spring Boot JDBC + MySQL + HikariCP example

In this article, we will show you how to create a Spring Boot JDBC application + MySQL and HikariCP.

Tools used in this article :

1. Spring Boot 1.5.16.RELEASE
2. MySQL 5.7.x
3. HikariCP 2.6
4. Maven
5. Java 8
6. IntelliJ IDEA Ultimate 2018.2



```java
mvn clean package
java -jar target/spring-boot-jdbc-1.0.jar
```

```
java -Dspring.datasource.initialize=false -jar target/spring-boot-jdbc-1.0.jar insert newUser newPassword
```

DATASOURCE = HikariDataSource (HikariPool-1)

[Usage] java xxx.jar {insert name email | display}

DATASOURCE = HikariDataSource (null)

Add customer...

Done!

```
java -Dspring.datasource.initialize=false -jar target/spring-boot-jdbc-1.0.jar display
```

```
DATASOURCE = HikariDataSource (null)
Display all customers...
Customer{id=1, name='hendisantika', email='111@yahoo.com', date=2017-03-24}
Customer{id=2, name='naruto', email='222@yahoo.com', date=2017-03-24}
Customer{id=3, name='kakashi', email='333@yahoo.com', date=2017-03-24}
Customer{id=4, name='newUser', email='newPassword', date=2017-03-24}
Done!
```
