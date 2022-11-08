---
title: "[Spring] Project"
author: Jiwonss
categories: [Spring]
tags: [spring]
---

## 1. 프로젝트 생성

Spring Boot

[Spring Initialzr](https://start.spring.io/)

## 2. 프로젝트 설정

Gradle

## 3. 프로젝트 실행

### SpringTestApplication.java

{: file='SpringTestApplication.java'}

```java
@SpringBootApplication
public class SpringTestApplication {

	public static void main(String[] args) {
		SpringApplication.run(SpringTestApplication.class, args);
	}

}
```

### main.html

{: file='main.html'}

```html

```

### PageController.java

{: file='PageController.java'}

```java
@Controller
public class PageController {

}
```

```java
// 1
@GetMapping("/")
public String main() {
    return "main";
}

// 2
@GetMapping("/")
public ModelAndView main(){
    return new ModelAndView("main");
}
```
