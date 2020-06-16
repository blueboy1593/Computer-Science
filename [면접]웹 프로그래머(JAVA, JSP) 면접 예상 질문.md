# [면접]웹 프로그래머(JAVA, JSP) 면접 예상 질문

보통의 프로그래밍 면접에서 빈출하는 지식들 정리한 것.

1. JAVA

   자바는 네트워크상에서 쓸 수 있도록 미국의 선 마이크로 시스템즈가 개발한 객체 지향 프로그래밍 언어

   - 자바가상머신(JVM)만 설치하면 운영체제에 상관없이 작동(운영체제에 독립적)
   - 기본 자료형 제외 모든 요소들이 객체로 표현
   - 캡슐화, 상속, 다형성이 잘 적용된 언어
   - Garbage Collector를 통해 자동적인 메모리 관리
   - 멀티쓰레드(Multi-thread) 지원

2. OOP(객체 지향 프로그래밍)

   Object Oriented Programming

   데이터를 객체로 취급하여 프로그래밍에 반영, 순차적 기존의 것들과 달리 객체의 상호작용으로 프로그램이 동작

   - 코드의 재사용성이 높다
   - 코드의 변경이 용이
   - 직관적인 코드분석 가능
   - 개발속도 향상
   - 상속을 통한 장점 극대화

3. Object

   같은 성질, 같은 구조와 형태를 가지는 객체는 등급으로 정의

   등급에 속하는 객체는 등급의 인스턴스
   
4. Overloading vs Overriding
   

Overloading

   - 같은 이름의 메소드를 여러개 정의하는 것
   - 매개변수의 타입이 다르거나 개수가 달라야 한다

   Overriding

   - 상속에서 나온 개념
   - 상위 클래스(부모 클래스)의 메소드를 하위 클래스(자식 클래스)에 재정의

5. Servlet, JSP

   Servlet - Container가 이해할 수 있게 구성된 순수 자바 코드로만 이루어진 것(Html in JAVA)

   JSP(Java Server Page) - html 기반에 JAVA코드를 블록화하여 삽입한 것(JAVA in Html)

6. JDBC

   Java Data Base Connection

   JAVA 언어로 데이터 베이스에 접근할 수 있는 프로그래밍

7. GET / POST

8. Session / Cookie

   HTTP 프로토콜을 이용하는 웹사이트에서 머무르는 동안 방문자의 상태를 저장하기 위해 사용함

   Session

   - 서버에 저장됨
   - 쿠키에 비해 보안성이 좋다

   Cookie

   - Client PC에 저장됨
   - 다른 사용자에 의해서 임의로 변경이 가능하다

   Session에 모두 저장하면 Server의 메모리를 과도하게 사용하게 되어 Server에 무리가 감.

9. MVC 패턴

   사용자 인터페이스를 성공적이며 효과적으로 데이터 모형에 관련 시키기 위한 방법론 or 설계 방식

   목적 코드의 재사용에 유용한 것은 물론 개발에 소요되는 시간을 현저하게 줄여주는 형식.

   Model - 논리적 데이터 기반 구조를 표현. (사용자 인터페이스 정보 X)

   View - 사용자 인터페이스 내의 구성요소를 표현(사용자에게 보여지는 화면)

   Controller - Model과 View를 연결하고 있는 클래스를 대표. 정보교환

10. Interface, Abstract

    일단 이 친구들은 잘 모르겠어.

    상속과 추상이 키워드인 것 같고.

    - 프로토타입만 있는 메서드를 갖는다.
    - 하위클래스에서 확장/ 구현 해야 한다.

11. Call by Reference / Call by Value

    Call by Reference

    - 매개 변수의 원래 주소에 값을 저장
    - 클래스 객체를 인수로 전달한 경우

    Call by Value

    - 인수로 기본 데이터형을 사용.
    - 주어진 값을 복사하여 처리하는 방식
    - 메서드 내의 처리 결과는 메서드 밖의 변수에 영향을 X

12. Static

    - 클래스 로딩시 메모리 공간 할당.
    - 처음 설정된 메모리 공간이 변하지 않음
    - 객체를 아무리 많이 만들어도 해당 변수는 하나만 존재.

13. Framework

14. Garbage Collection(가비지 콜렉션)

    - 더이상 사용하지 않는 동적 할당된 메모리 블럭을 찾아 자동으로 다시 사용 가능한 자원으로 회수
    - 가비지 컬렉터

15. Primitive type / Reference type

    Primitive type

    변수에 값 자체를 저장

    - 정수형
    - 실수형
    - 문자형
    - 논리형

    Wrapper Class를 통해 객체로 변형

    Reference type

    메모리상에 객체가 있는 위치를 저장

    - Class
    - Interface
    - Array

16. Wrapper Class

    Primitive type으로 표현할 수 있는 간단한 데이터를 객체로 만들어야 할 경우 기능 지원

17. Spring Framework(스프링 프레임워크)

    오픈소스임

    - 크기와 부하의 측면에서 경량
    - 제어 역행(IoC)라는 기술을 통해 느슨한 결합을 도모
    - 관점지향 프로그래밍(AOP)을 위한 풍부한 지원
    - 확장성이 높다

18. Thread
    
    Thread - 프로세스내에서 동시에 실행되는 독립적인 실행 단위
    
    - 자원을 많이 사용하지 않음
    - 구현이 쉽다
    - 범용성이 높다
    
    Process(프로세스) - 운영체제에서 실행중인 하나의 프로그램(하나 이상의 쓰레드)
    
    Thread 장점
    
    - 빠른 프로세스 생성
    - 적은 메모리 사용
    - 쉬운 정보 공유
    
    Thread 단점
    
    - 교착 상태에 빠질 수 있다.
    
    교착상태 - 하나 or 이상의 프로세스가 수행할 수 없는 어떤 특정시간을 기다리고 있는 상태
    
19. 접근제한자(Public > protected > default > private)

    public - 접근 제한이 없다

    protected - 같은 패키지 내, 다른 패키지에서 상속받아 자손클래스에서 접근 가능

    default - 같은 패키지 내에서만 접근 가능

    private - 같은 클래스 내에서만 접근 가능

20. 소켓 통신(TCP / UDP)

    Transmission Control Protocol

    - 연결형 서비스 제공
    - 높은 신뢰성 보장
    - 연결의 설정(3-way handshaking)
    - 연결의 해제(4-way handshaking)
    - 데이터 흐름 제어, 혼잡 제어
    - 전이중, 점대점 서비스(양방향 송수신 서비스)

    User Datagram Protocol

    - 비연결형 서비스 제공
    - 신뢰성 낮음
    - 데이터의 전송 순서 바뀔 수 있음
    - 데이터 수신 여부 확인 X
    - TCP보다 빠른 전송속도

21. Stack / Queue

    Stack

    - Last in First Out 후입선출
    - push()로 데이터 입력, pop()로 데이터 출력
    - 역순 문자열 만들기, 수식의 괄호 검사, 수식의 후위 표기법 변환 등에 사용

    Queue

    - First In First Out 선입선출
    - enQueue()를 이용한 데이터 입력, deQueue()를 이용한 데이터 출력
    - Linear Queue(선형큐)는 메모리 재사용이 불가능
    - Circular Queue(원형큐)는 이를 보완함

22. Singleton Design Pattern

    클래스 인스턴스가 하나만 만들어지도록 하고, 그 인스턴스에 대한 전역 접근을 제공한다.

23. Database에서 Index의 역할은?

    Index

    - 테이블에 대한 동작의 속도를 높여주는 자료 구조
    - 검색을 빠르게 할 수 있다

24. DB에서 자료를 검색하는 두 가지 방법

    FTS(Full Table Scan) : 테이블을 처음부터 끝까지 검색하는 방법

    Index Scan : 인덱스를 검색하여 해당 자료의 테이블을 액세스 하는 방법.



출처: https://hahahoho5915.tistory.com/16 [넌 잘하고 있어]