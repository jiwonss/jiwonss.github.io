---
title: "[Spring] Project"
author: Jiwonss
categories: [Spring]
tags: [spring]
---

## 1. 프로젝트 생성

Spring Boot

[Spring Initialzr](https://start.spring.io/)에서 프로젝트 생성

## 2. 프로젝트 실행

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

	@GetMapping("/")
	public String main() {
		return "main";
	}

}
```

{: file='PageController.java'}

```java
@Controller
public class PageController {

	@GetMapping("/")
	public ModelAndView main(){
		return new ModelAndView("main");
	}

}
```
