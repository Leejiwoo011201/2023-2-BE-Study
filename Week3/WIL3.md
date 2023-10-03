# 1. Spring Bean이란 무엇인가?

스프링 IoC 컨테이너에 의해 관리되는 자바 객체

# 2. Spring Bean을 등록하는 방법을 정리하라

> 1. JavaConfig를 사용한 Spring Bean 등록
>   
>   @Configuration 어노테이션을 클래스에 붙여서 클래스를 정의.
>   
> 
>         그 후, Spring Bean을 정의하는 메서드에 @Bean 어노테이션을 붙임.
> 
>         밑 코드는 위 방식의 예시 코드.
> 
> ```java
> public class AppConfig { // JavaConfig를 사용하여 Bean 등록 
>     @Bean public MyBeanClass myBean() 
>         { return new MyBeanClass();
>      }
> }
> ```

> 2. Component Scanning
> 
> Spring 구성 클래스에서 @ComponentScan, @Component 어노테이션을 사용

위 2가지 방법으로 Spring Bean 등록이 가능하다
