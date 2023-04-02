# Week2 WIL 

https://www.notion.so/WEEK2-302ee9f1d338417ab6c6e64f52e8b140?pvs=4


### 일반적인 웹 어플리케이션의 계층 구조

**컨트롤러 + 서비스 + 리포지토리 + 도메인**

## **컨트롤러 (Controller)**

**→ 웹 MVC의 컨트롤러 역할**

**→ 쉽게 말하자면 사용자의 요청에 따른 응답을 알려주는 역할이다.**

**→ 사용자의 요청을 받아 처리 데이터와 UI를 연결한다.** 

## **서비스 (Service)**

**→ 핵심 비즈니스 로직 구현** 

**예시) 중복 가입 불가 등**

**→ 컨트롤러에서도 비즈니스 로직 구현이 가능하나 비즈니스 로직의 재사용 및 유지보수를 위해 분리하여 서비스에 구현한다.**

**→ MVC에서 Model이 데이터베이스에서 받아온 데이터를 전달받아 가공하는 역할을 한다.**

## **리포지토리 (Repository)**

**→ 데이터 베이스에 접근, 도메인 객체를 데이터베이스에 저장하고 관리한다.**

## **도메인 (Domain)**

**→ 비즈니스 도메인 객체**

**→ 회원, 주문, 쿠폰 등등 주로 데이터베이스에 저장하고 관리된다.**

# **TDD(Test Driven Development)**

**→ 테스트 주도 개발로 소프트웨어 개발 방법론 중 하나**

**→ 개발 후 테스트 방식이 아닌 테스트 후 개발 방식의 프로그래밍 방법이다**

## **TDD의 필요성**

**→ test는 공유가 쉽기 때문에 타인의 코드에 쉽게 접근 가능하고, 이해가 빨라지므로 협업 및 협력에 좋다.**

**→ 문제가 발생하였을 때 모듈별로 테스트를 진행하면 문제 지점을 쉽게 찾을 수 있어 유지보수에 용이하다.**

**→ 유지보수(리팩토링) 과정에서 중복된 코드들은 제거되고, 복잡한 코드들은 정리되면서 코드를 깔끔하게 작성할 수 있고, 장기적으로는 개발 비용을 절감할 수 있다.**



**구글링 출처**

[https://sowon-dev.github.io/2020/10/18/201019spring/](https://sowon-dev.github.io/2020/10/18/201019spring/)


[https://wikidocs.net/160890](https://wikidocs.net/160890)

[http://clipsoft.co.kr/wp/blog/tddtest-driven-development-방법론/](http://clipsoft.co.kr/wp/blog/tddtest-driven-development-%EB%B0%A9%EB%B2%95%EB%A1%A0/)

[http://www.incodom.kr/테스트_주도_개발](http://www.incodom.kr/%ED%85%8C%EC%8A%A4%ED%8A%B8_%EC%A3%BC%EB%8F%84_%EA%B0%9C%EB%B0%9C)
