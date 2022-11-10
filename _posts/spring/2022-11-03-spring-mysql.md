---
title: "[Spring] MySQL"
author: Jiwonss
categories: [Spring]
tags: [spring]
---

## 1. MySQL

### MySQL

```sql
-- database 생성
create database spring_test;

-- user 생성
create user 'springtest'@'%' identified by '{ password }';

-- 권한 부여
grant all on spring_test.* to 'springtest'@'%';
```

### application.yml

{: file='application.yml'}

```yml
spring:
  datasource:
    url: jdbc:mysql://localhost:3306/spring_test
    username: springtest
    password: { password }
    driver-class-name: com.mysql.cj.jdbc.Driver

  jpa:
    hibernate:
      ddl-auto: update
```

## 2. MySQL Test

### SpringTestEntity.java

{: file='SpringTestEntity.java'}

```java
@Data
@Entity
@Table(name = "spring_test")
public class SpringTestEntity {

    @Id
    @GeneratedValue(strategy = GenerationType.IDENTITY)
    private Long id;

    private String title;

    private String content;

}
```

### SpringTestRepository.java

{: file='SpringTestRepository.java'}

```java
public interface SpringTestRepository extends JpaRepository<SpringTestEntity, Long> {

}
```

### SpringTestRestController.java

{: file='SpringTestRestController.java'}

```java
@RestController
@RequestMapping("/api")
public class SpringTestRestController {

    @Autowired
    private SpringTestRepository springTestRepository;

    @GetMapping
    public List<SpringTestEntity> findAll() {
        return springTestRepository.findAll();
    }

    @PostMapping
    public SpringTestEntity add(@RequestBody SpringTestEntity springTestEntity) {
        return springTestRepository.save(springTestEntity);
    }

}
```

### Postman

|          |                           |     |
| -------- | ------------------------- | --- |
| **POST** | http://localhost:8080/api | Add |

```json
{
  "title": "test",
  "content": "test입니다."
}

{
  "title": "test2",
  "content": "test2입니다."
}
```

|         |                           |          |
| ------- | ------------------------- | -------- |
| **GET** | http://localhost:8080/api | Find All |

{: file='response'}

```json
[
  {
    "id": 1,
    "title": "test",
    "content": "test입니다."
  },
  {
    "id": 2,
    "title": "test2",
    "content": "test2입니다."
  }
]
```

![Result](/assets/img/spring/mysql-test-result.png){: w="700" h="400" }
