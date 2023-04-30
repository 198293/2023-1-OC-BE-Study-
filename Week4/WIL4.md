# Week4

**WEEK4 WIL**

[https://www.notion.so/Week4-fa236a8f9da74ef48086c3bb8e61f66f?pvs=4](https://www.notion.so/Week4-fa236a8f9da74ef48086c3bb8e61f66f)

# **< 필수 정리 내용 >**

## 1. **순차 지향 프로그래밍과 절차 지향 프로그래밍의 특징과 차이**

### 순차지향 프로그래밍(****Procedural Programming)****

**= 절차지향 프로그래밍**

**→ 알고리즘의 프로세서가 일련의 절차에 의해  돌아가게 되는 프로그래밍** 

**[장점]**

- **객체지향 프로그래밍 보다 알고리즘 처리 속도가 빠르다.**

**[단점]**

- **유지보수가 어렵다는 점입니다.**

**→ 프로그램 전체가 한 덩어리이기 때문에 알고리즘이 복잡해지고 길어질수록 수정하려면 전체를 다 봐야하고 알고리즘이 꼬일 수 있다.**

- **코드의 순서가 바뀌면 동일한 결과를 보장하기 어렵습니다.**

**→ 실행 순서가 정해져 있기 떄문이다**

- **디버깅이 어렵습니다.**

### **객체지향 프로그래밍(Object Oriented Programming)**

**→ 데이터와 절차를 하나의 덩어리로 묶어 하나 하나 각각을 객체를 마치 부품처럼 만들어 조립하고 운영하는 알고리즘**

**→ 문제의 요소들을 객체로 모델링해서, 클래스의 특징인 캡슐화, 상속성, 다형성을 이용해 풀어가는 과정을 가진다.**

**→ 객체지향 언어는 절차지향 언어의 단점을 보완하고자 등장하였지만 무조건 적으로 우수하다고 할 수는 없다.**

- **캡슐화로 결합도를 낮추고 응집도를 높일 수 있다.**
- **상속 및 다형성을 통해 확장성과 코드의 재사용성이 높다**
- **추상화 및 다형성을 통해 유연한 설계와 복잡도 관리가 가능하다.**

**[장점]**

- **신뢰성 있는 소프트웨어를 쉽게 작성할 수 있다**
- **코드 재사용이 쉽다.**
- **업그레이드 및 디버깅이 쉽다.**
- **모듈을 재활용하기 때문에 하드웨어의 처리양을 줄여준다**
- **개발하려는 것을 기능별로 묶어 모듈화를 함으로써 하드웨어가 같은 기능을 중복으로 연산하지 않도록 한다.**

**[단점]** 

- **설계에 많은 시간을 투자해야 된다.**
- **상속관계의 부모클래스에서 버그가 일어나면 자식 클래스에서 정상 동작인지 예측이 어렵고, 자식  클래스의 기능이 변경될 수 있다.**

## 2. **JVM의 역할과 가비지컬렉션(GC)이란?**

### **JVM(Java Virtual Machine)이란?**

**→ JVM은 Java Virtual Machine, 즉 자바 가상 머신의 약자를 따서 줄여 부르는 용어이다.** 

**→ JVM은 OS와 Java 애플리케이션 사이의 중개자 역할을 한다.** 

**→ JVM은 자바 바이트코드를 실행할 수 있는 환경을 제공해주고 이를 통해 자바 바이트 플랫폼에 독립적으로 어디서든 실행될 수 있게 한다. JVM을 통해 OS에 상관없이 어디서든 JAVA 애플리케이션을 실행할 수 있다.**

**→ JVM에는 Garbage Collecter(가비지 컬렉터)가 존재한다. Garbage Collecter는 더 이상 참조되지 않는 Garbage(가비지)라고 불리는 불필요한 메모리를 알아서 정리해주는 역할을 한다.** 

### 가비지 컬렉션 (Garbage Collection)이란?

→  **Garbage Collecter가 주기적으로 메모리 누수를 방지하기 위해 메모리를 청소하는 과정을 Garbage Collection(GC)라고 한다.**

**→ Garbage Collection(GC)은  메모리 공간을 확보하고 메모리 누수(memory leak)을 막는 역할을 한다.** 

**→ C, C++에서는 Garbage Collection(GC)이 없어 개발자가 메모리 할당과 해제를 직접 해주어야 하지만, Java는 JVM에 탑재되어 있는 Garbage Collecter가 메모리를 자동으로 관리해준다.**

## 3. **메소드, 힙, 스택 영역에 각각 어떤 게 존재하는가?**

![img1.daumcdn.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/795b00ff-1d7b-4a18-9afe-f447bad04c68/img1.daumcdn.png)

### **메소드(Method) 영역**

**=  Static 영역** 

**→ 전역 변수와 정적 멤버변수(static 변수)가 저장되는 영역.**

**→ 메인 메소드에서 사용하는 클래스와 static 변수는 메소드 영역에 저장된다.** 

### **스택 (Stack) 영역**

**→ 지역변수, 매개변수, 인자값, 리턴값이 저장되는 영역**

**→ 메소드 안에서 사용되는 기본형 변수들이 값과 함께 저장되고 Heap 영역에 생성된 객체들을 참조하는 주소값이 할당된다.**

**→ 스택 영역에는 프로그램의 실행 과정에서 임시로 할당되는 곳이기 때문에 메소드 호출할 때마다 저장하고, 메소드 호출이 끝나면 메소드를 위해 준비했던 변수들이 스택에서 제거된다.**

**+**

**지역변수 - 오컬 변수, 메소드 안에서 선언한 변수**

**매개변수 - 파라미터 변수, 메소드를 선언할 때 argument 안에 넣는 변수**

**→ 두 변수 모두 선언된 블록 안에서만 유효하기 때문에 스택영역에 저장한다.**

### **힙(Heap) 영역**

**→ JAVA 프로그램에서 사용되는 모든 인스턴스 변수(객체)들이 저장되는 영역**

**(자바에서는 new를 사용하여 객체를 생성하면 힙 영역에 저장된다.)** 

**→ 힙 영역은 메모리 공간이 동적으로 할당되고 해제되며 메모리의 낮은 주소에서부터 높은 주소로 할당이 이루어집니다.**

**→ 스택 영역과 다르게 메소드 호출이 끝나도 제거되지 않는다.**

**→ 주소를 잃어버려 Garbage가 되어 Garbage Collecter에 의해 지워지거나, JVM이 종료될 때까지 저장된다.**

**8개 타입 이외의 변수로 저장된 레퍼런스 변수들은 자주 호출되어 사용하기 떄문에 스택 영역에 주소를 저장하고, 힙 영역에 실제 변수의 값을 저장한다.**

## 4. “**클래스는 붕어빵 틀이고 객체는 붕어빵이다.” 에 대해서 논하시오.**

![images.jpg](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f92905d9-90be-440f-ac37-6dc07af1813c/images.jpg)

- **클래스 : 분류. 집합. 같은 속성과 기능을 가진 객체를 총칭하는 개념으로 분류에 대한 개념이다.**

- **객체: 세상에 존재하는 유일무이한 사물로 실체이다**

> **클래스 : 객체 = 사람 : 홍길동 = 붕어빵 틀 : 붕어빵**
> 

→ **클래스는 객체의 설계도라고 하기 떄문에  “클래스는 붕어빵 틀이고 객체는 붕어빵이다.”라는 표현을 사용한다.**

# **<선택 정리 내용>**

[data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==](data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==)

### **[1~3] O/X 중 고르시오.**

### 1. 절차지향 프로그래밍은 객체지향 프로그래밍의 반대 개념이다. (X)

![image.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/82def36d-569a-4e16-92f2-76440e35e65c/image.png)

- **절차지향은 순차적으로 실행에 초점을 둔다**

→ **명령어가 순차적으로 주기억장치에 들어가기 때문에 객체지향보다 빠른 속도를 낼 수 있다.**

- **객체지향은 객체간의 관계/조직에 초점을 둔다**

### 2. 절차지향과 객체지향을 구분하는 방법으론 “상속, 다형성의 유무”가 있다. (O)

**→ 객체 지향은 추상화, 캡슐화, 상속, 다형성을 골고루 사용해 프로그래밍하는 방법이기 때문에 상속, 다형성의 유무를 통해 절차지향 프로그래밍과 객체지향 프로그래밍을 구분할 수 있다.**

### 3. 다음 상황에 대해 답하시오.

### (1) a와 b는 모두 스택 메모리 영역에 저장 공간을 확보한다. (X)

**→ a와 b는 객체 타입(Integer)이므로, heap 메모리 영역에 저장된다.** 

**객체 타입의 변수는 해당 객체가 저장되어 있는 heap 메모리의 주소값을 참조(reference)하므로, 변수 자체가 저장되는 스택 메모리 영역과는 다르다. 이렇게 저장된 변수는 필요에 따라 해당 객체의 값을 변경하거나 다른 객체를 참조할 수 있습니다.**

### (2) a.equals(b) 는 참이다. (X)

### (3) a == b 는 참이다. (X)

**→ 자바에서 -128부터 127까지의 정수 값에 대해서는 캐싱을 하기 때문에, a와 b가 128보다 작은 정수 값을 참조하고 있다면, 두 변수가 같은 객체를 참조할 수 있다. 이 경우 a == b, a.equals(b)는 true를 반환한다. 500은 해당 범위를 벗어나는 정수이므로, a와 b는 서로 다른 객체를 참조한다. 따라서** 

**a == b와 a.equals(b)는 false를 반환한다.**

[data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==](data:image/gif;base64,R0lGODlhAQABAIAAAP///wAAACH5BAEAAAAALAAAAAABAAEAAAICRAEAOw==)

### **[4~5] 다음 질문에 답하시오.**

### 4. 객체지향 프로그래밍의 단점은 무엇인가? (성능과 설계 측면에서 각각 서술하시오.)

→  **성능적인 측면에서의 단점:
객체지향 프로그래밍은 객체 간의 상호작용이 많이 일어나기 때문에, 메모리 및 처리 성능의 부담이 발생할 수 있다. 또한 객체지향 프로그래밍에서는 추상화나 다형성 등의 기능을 사용하기 위해 추가적인 메모리와 연산이 필요하므로 성능이 저하될 가능성이 있다.**

→ **설계 측면에서의 단점:
객체지향 프로그래밍에서는 상속, 캡슐화 등의 개념을 이용해 코드를 구조화하므로, 이를 적절하게 사용하지 않으면 복잡한 코드 구조가 발생할 수 있다. 또한 객체지향 프로그래밍에서는 클래스 간의 의존성이 높아져 변경 사항이 발생했을 때 유지보수가 어려울 수 있다. 객체 간의 의존성이 높아질 경우에는 코드 재사용이 어려울 수 있다.**

### 5. 객체와 클래스의 차이는 무엇인가?

![download.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/39e936ce-52a7-404f-bdc2-061c828c7f43/download.png)

- **클래스(Class) : 분류. 집합. 같은 속성과 기능을 가진 객체를 총칭하는 개념으로 분류에 대한 개념이다.**

- **객체(Object) : 세상에 존재하는 유일무이한 사물로 실체이다**

→ **클래스(Class)는 객체를 생성하기 위한 설계도로 객체의 속**

**성과 행위를 정의하는 데에 사용된다. 클래스는 여러 개의 객체를 생성할 수 있고, 이러한 객체는 클래스의 인스턴스(instance)이다.** 

**→ 객체는 클래스에서 정의한 멤버 변수와 멤버 함수를 가지며, 이를 통해 객체의 상태와 행위를 표현할 수 있다. 객체는 각자의 고유한 상태와 행위를 가지며, 다른 객체와 구분될 수 있습니다.**

**[출처]**

 [절차지향언어 vs 객체지향언어](https://blog.naver.com/gitacademy01/222394033958)|

[https://luminousblog.tistory.com/24](https://luminousblog.tistory.com/24)

[https://usefultoknow.tistory.com/entry/절차지향Procedural-Programming-객체지향Object-Oriented-Programming-장단점-및-차이점](https://usefultoknow.tistory.com/entry/%EC%A0%88%EC%B0%A8%EC%A7%80%ED%96%A5Procedural-Programming-%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5Object-Oriented-Programming-%EC%9E%A5%EB%8B%A8%EC%A0%90-%EB%B0%8F-%EC%B0%A8%EC%9D%B4%EC%A0%90)

[https://velog.io/@sejin3319/OOP절차지향-프로그래밍-객체지향-프로그래밍](https://velog.io/@sejin3319/OOP%EC%A0%88%EC%B0%A8%EC%A7%80%ED%96%A5-%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D-%EA%B0%9D%EC%B2%B4%EC%A7%80%ED%96%A5-%ED%94%84%EB%A1%9C%EA%B7%B8%EB%9E%98%EB%B0%8D)

[https://code-lab1.tistory.com/92](https://code-lab1.tistory.com/92)

[https://devfunny.tistory.com/681](https://devfunny.tistory.com/681)

[https://chunsubyeong.tistory.com/76](https://chunsubyeong.tistory.com/76)

[https://coding-factory.tistory.com/830](https://coding-factory.tistory.com/830)

[https://pearlluck.tistory.com/10](https://pearlluck.tistory.com/10)
