# Week3 WIL

https://www.notion.so/Week3-74a94d0c392643db99d6f6beeb5e9496?pvs=4


[https://www.gdschongik.com/backend-study/subject/3](https://www.gdschongik.com/backend-study/subject/3)

## **의존성(Dependency)**

→ **파라미터나 리턴값 또는 지역변수 등으로 다른 객체를 참조하는 것을 의미한다.**

**→ 의존성은 객체 간의 협력을 위해 필수적이다.**

**→ 하지만 위험하기 때문에 의존성은 최소화되어야 한다. 한 객체가 다른 객체에 의존한다는 것은 다른 객체가 변할 때 변경이 전파될 수 있다는 것을 의미하기 때문**

## **@Autowired 의존성 주입**

**→ spring에서 제공하는 의존성 주입 방법**

**→ 의존성 주입은 필요한 객체를 직접 생성하는 것이 아닌 외부로부터 객체를 받아 사용하는 것**

**== 이를 통해 객체간의 결합도를 줄이면서 코드를 유연하게 작성할 수 있고, 코드의 재활용성을 높일 수 있다.**

## **의존성 주입의 3가지 방법**

**1. 생성자 주입(Constructor Injection)**

**2. 필드 주입(Field Injection)**

**3. 수정자 주입(Setter Injection)**

→ **Spring Framwork reference에서 권장하는 방법은 생성자를 통한 주입**

## **DIP(Dependency Inversion Principle) == 의존성 역전 원칙**

![img1.daumcdn.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a6ef4770-6b6d-4f39-acce-72506bd10208/img1.daumcdn.png)

**→ 객체에서 어떤 Class를 참조해서 사용해야하는 상황이 생긴다면, 그 Class를 직접 참조하는 것이 아니라 그 대상의 상위 요소(추상 클래스 or 인터페이스)로 참조하라는 원칙이다.**

1. **상위 모듈은 하위 모듈에 의존해서는 안된다.**
2. **추상화는 세부 사항에 의존해서는 안된다**

**장점**

- **확장성이 용이하다!**
- **객체간의 관계를 최대한 느슨하게 해준다. →  다양한 설계 방식, 혹은 복잡한 시스템 설계가 가능하게 된다.**

## **스프링 빈이란?**

**→ Spring 컨테이너에 의하여 관리되는 자바 객체를 의미한다.**

**→ 컴포넌트 스캔은 @Component를 명시하여 빈을 추가하는 방법이다. 클래스 위에 @Component를 붙이면 스프링이 알아서 스프링 컨테이너에 빈을 등록한다.**

## **스프링 컨테이너란?**

**→ 스프링 컨테이너는 스프링 빈의 생명 주기를 관리하며, 생성된 스프링 빈들에게 추가적인 기능을 제공하는 역할을 한다.**

**→ SQL문을 직접 java application내에서 적을 경우가 적어진다는 장점이 존재한다.**

## **JPA(Java Persistent API)**

![4sVPQ.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/dc78bbd4-5025-444e-a134-a8ee578c3159/4sVPQ.png)

**→ 직접적인 SQL 문을 사용하지 않고 자바 코드를 사용해서 DB에 접근, 조작할 수 있는 기술.** 

→ **JPA 역시 내부적으로 JDBC를 사용한다.**

## **JDBC(Java Database Connectivity)**

![JDBC 구조.webp](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/15d3c072-9ed4-42ec-acde-bb7393eed2e4/JDBC_%EA%B5%AC%EC%A1%B0.webp)

**→ DB에 접근(Connectivity)할 수 있도록 Java에서 제공하는 API.**

**→ JPA를 사용할 경우 많은 장점이 있지만 어렵고 제대로 사용하지 않을 경우 데이터 손실이 있다는 단점이 있다.**

**선택 정리 내용**

## **@GetMapping(”hello”)**

**→ [localhost:8080](http://localhost:8080)에 접속하면 (아래 터미널에 링크 주소 나타남. ) hello가 화면에 뜨는 것을 확인할 수 있다.**

**→ HTTP Method인 Get의 요청을 받을 수 있는 API를 만들어주는 어노테이션이다.**

## **model은 어떤 용도로 쓰는가?**

**→ Controller의 메서드는 Model이라는 타입의 객체를 파라미터로 받을 수 있다.**

**→ Model 객체는 컨트롤러에서 데이터를 생성해 이를 JSP 즉 View에 전달하는 역할**

**→ "addAttribute"를 통해 View로 데이터를 전달할 수 있습니다. ⇒  [localhost](http://localhost:8080)에서 확인 가능**

## **return “hello”; 를 하는 이유**

**→ hello라는 객체를 생성해주고, 해당 객체를 리턴하여 나타내면 json방식으로 나오는 것을 확인할 수 있다.**

## **@ResponseBody**

**→ 자바객체를 HTTP요청의 바디내용으로 매핑하여 클라이언트로 전송한다.**

**→ @ResponseBody 의 의미는 http 통신 프로토콜의 응답 body 부분에 데이터를 직접 넣어주겠다는 의미.** 

→ **기존 탬플릿 엔진과의 차이는 View 없이 데이터가 그대로 전달된다.**

## **JPA(Java Persistence API)**

![img1.daumcdn.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6345c988-2635-4772-ae96-0ba302012a6a/img1.daumcdn.png)

**→  Java 진영에서 ORM(Object-Relational Mapping) 기술 표준으로 사용하는 인터페이스 모음**

**→  JPA는 다양한 쿼리 방법을 지원한다 : JPQL, JPA Criteria, QueryDSL, 네이티브 SQL**

![img1.daumcdn.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f2e4a473-6061-4727-bbcf-c9261c8d9d1a/img1.daumcdn.png)

**→ JPA는 반복적인 CRUD SQL을 처리해준다.**

**→ SQL아닌 객체 중심으로 개발할 수 있다.**

**→ 생산성이 좋아지고 유지보수도 수월하다.**

## **jpql (Java Persistence Query Language)**

**→ 가장 단순한 조회 방법 ⇒ 검색을 할 때도 테이블이 아닌 엔티티 객체를 대상으로 검색**

**→  문법이 SQL과 비슷하다**

**구글링 출처**

[https://mangkyu.tistory.com/226](https://mangkyu.tistory.com/226)

[https://dev-coco.tistory.com/70](https://dev-coco.tistory.com/70)

[https://huisam.tistory.com/entry/DIP](https://huisam.tistory.com/entry/DIP)

[https://inpa.tistory.com/entry/OOP-💠-아주-쉽게-이해하는-DIP-의존-역전-원칙](https://inpa.tistory.com/entry/OOP-%F0%9F%92%A0-%EC%95%84%EC%A3%BC-%EC%89%BD%EA%B2%8C-%EC%9D%B4%ED%95%B4%ED%95%98%EB%8A%94-DIP-%EC%9D%98%EC%A1%B4-%EC%97%AD%EC%A0%84-%EC%9B%90%EC%B9%99)

[https://blog.naver.com/boldfaced7/223066835433](https://blog.naver.com/boldfaced7/223066835433)

[https://steady-coding.tistory.com/594](https://steady-coding.tistory.com/594)

[https://sowon-dev.github.io/2021/03/22/210323jpaVSjdbc/](https://sowon-dev.github.io/2021/03/22/210323jpaVSjdbc/)

[https://unit-15.tistory.com/148](https://unit-15.tistory.com/148)

[https://gocoder.tistory.com/2489](https://gocoder.tistory.com/2489)

[https://soom-soom.tistory.com/172](https://soom-soom.tistory.com/172)

[https://cheony-y.tistory.com/329](https://cheony-y.tistory.com/329)

[https://dbjh.tistory.com/77](https://dbjh.tistory.com/77)
