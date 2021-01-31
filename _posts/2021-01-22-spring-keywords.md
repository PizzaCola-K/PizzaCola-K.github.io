---
title: Java Spring Keyword
date: 2021-01-31 08:57:00 +0900
categories: [Keywords]
tags: [spring]     # TAG names should always be lowercase
---

# 디자인 패턴 (스프링)

- 어댑터 패턴
- 프록시 패턴
- 데코레이터 패턴
- 싱글턴 패턴
- 템플릿 메서드 패턴
- 팩터리 메서드 패턴
- 전략 패턴
- 템플릿 콜백 패턴
- 프론트 컨트롤러 패턴
- MVC 패턴

# Spring Triangle

- Inversion of Control / Dependency Injection
- AOP Aspect oriented Programming
- PSA Portable Service Abstract

# IoC

- IoC [IoC](https://martinfowler.com/articles/injection.html)
- IoC Container [IoC Container](https://docs.spring.io/spring-framework/docs/current/reference/html/core.html#beans)
- Bean

- ApplicationContext
- @Autowired
- @Component / @ComponentScan
- InitializingBean / DisposableBean
  - @Bean(initMethod / destoryMethod)

- @Scope("prototype"/"singleton")
  - prototype은 lifecycle이 조금 다름

# AOP

- 컴파일 (AspectJ)
- 바이트코드 조작 (AspectJ)
- 프록시 패턴 (Spring AOP) [Design-pattern](https://refactoring.guru/design-patterns/proxy)

- Advice
  - Before
  - After Returning
  - After Throwing
  - After
  - Around

- Joinpoint
- Pointcut
- Weaving
- Aspect

# PSA

- Transaction ... 