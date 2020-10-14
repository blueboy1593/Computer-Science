# 18 하반기 공채 라인(Line) 1차 면접 답변 연습

출처 : goodGid님의 블로그

출처 URL : https://goodgid.github.io/18-Second-Half-Line-1st-Interview/

- 3:1 50분 면접
- 자기소개 / 재밌었던 수업 / 핀테크 지원이유
- 면접관분들은 각각은 다른 부서다.
- 편한 분위기로 진행해주셨다.
- 블로그 들어가서 글 보고 질문하셨다.
- 판서를 하진 않았는데 케바케이다.
- OS, Java 질문 x —> 내가 했던 프로젝트 기반으로 물어봤다. 이 또한 케바케다.

> 면접 시 받은 질문

- 개인적인 질문들은 최대한 배제하고 작성하였다.

Q. HTTP Method랑 REST API의 어떤 행위와 매칭이 되는가?

POST - Create

GET - Select

PUT - Update

Delete - Delete

Idempotent라는 한번 수행과 여러번 수행시의 결과가 같은지에 대해서는 POST만 X입니다.



Q. REST API의 특징은?

REpresentatiol State Transfer Application Programming Interface 의 약자입니다.

소프트웨어 프로그램 아키텍쳐의 한 형식입니다. 2000년도에 HTTP의 주요 저자인 로이 필딩이 당시 웹(HTTP) 설계의 우수성에 비해 제대로 사용되지 못하는 모습에 안타까워하며 장점을 최대한 활용할 수 있는 REST를 발표하였습니다.

자원 + 행위 + 표현

자원 : resource - URL

행위 : verb - HTTP method

표현 : representation

### 이점

1 ) 클라이언트 / 서버 구조로 나눌 수 있습니다. 

클라이언트는 유저 관련된 처리를, 서버는 REST api를 제공함으로써 각각의 역할이 구분되고 일관된 인터페이스로 작동합니다.

2) 무상태성 (Stateless)

3) 캐시 처리 가능(Cacheable)

4) 자체 표현 구조(Self-descriptiveness)

5) 계층화 (Layered System)

클라이언트와 서버가 구분되어 있기 때문에, 중간에 프록시 서버, 암호화 계층 등 중간매체를 사용할 수 있어 자유도가 높습니다.

6) 유니폼 인터페이스 (Uniform Interface)

HTTP 표준에만 따른다면 모든 플랫폼에서 사용이 가능하다. URI로 지정한 리소스에 대한 조작을 가능하게 하는 아키텍쳐 스타일



Q. RESTful이 무엇을 의미할까?

웹에 존재하는 모든 자원(이미지, 동영상, DB자원)에 고유한 URI를 부여해 활용하는 것으로, 자원을 정의하고 자원에 대한 주소를 지정하는 방법론을 의미합니다.



Q. URI vs URL의 차이는?

Uniform Resource Identifier / Uniform Resource Location

또다른 개념인 Uniform Resource Name이 있고, URI 안에 URL과 URN의 개념이 들어있습니다.

통합 자원 식별자로 인터넷에 있는 자원을 나타내는 유일한 주소입니다.

통합 자원 위치로 구분자.



Q. 프로젝트의 기술 스택은 어떻게 선정했어?

1) 프로젝트의 요구사항에 맞게

2) 하고싶은 기술 / 배워보고싶은 기술 등



Q. [Naver.com](http://naver.com/)을 들어가는 일련의 과정을 설명해줘



Q. 정적 파일을 빨리 받고 싶으면 어떻게 해야할까?

Q. JWT에 대해 설명해줘

JSON Web Token의 약자로, 두 개체에서 JSON객체를 사용하여 가볍고 자가수용적인 방식으로 정보를 안정성 있게 전달해줍니다. 대부분의 프로그래밍 언어에서 지원이 됩니다.

웹서버의 경우 HTTP의 헤더에 넣어서 전달 가능하고, URL의 파라미터로 전달 할 수 있습니다.

헤더 + 내용 + 서명 = header + payload + signature로 구성되어 있으며, parsing을 통한 해석, stringfy를 통한 암호화가 가능합니다.

해싱 알고리즘에는 HS256과 RSA를 자주 사용합니다.



Q. OAuth 1.0 / 1.1 / 2.0 의 차이를 이야기해 줘

OAuth는 인증을 위한 오픈 스탠더드 프로토콜로, 사용자가 Facebook이나 트위터 같은 인터넷 서비스의 기능을 다른 애플리케이션에서도 사용할 수 있게 한 것입니다.

2.0은 1.0과 호환되지 않고, 인증 절차가 간략하다는 장점이 있습니다.



Q. ID PW 이름 주민번호를 저장할 때 어떻게 해?

JSON형식으로 정보를 받아서 해싱알고리즘으로 토큰을 만들어서 하면 좋습니다.



Q. 암호화 방식에 대해 설명해줘

평문 : 해독 가능한 형태의 메세지

암호문 : 해독 불가능한 형태

암호화 : 평문을 암호문으로

복호화 : 암호문을 평문으로

대칭형 암호 vs 비대칭형 암호



Q. SSL 핸드쉐이킹은 어떻게 돌아가?

Secure Socket Layer이라는 뜻이고, Certificate Authority(CA)라고 불리는 써드 파티로부터 서버와 클라이언트의 인증을 하는데에 사용됩니다. 주로 전송계층과 응용계층 사이에서 보안조치를 하는데 사용합니다.

TLS(Transport Layer Security)로 최근에 불리며, SSL은 과거 명칭이라고 할 수 있습니다.



Q. 다른 언어 사용 경험은?

Python, Java, Javascript, Kotlin



Q. 프론트말고 백엔드가 좋은 이유는?

Q. DBMS는 어떤거 사용해봤어?

SQLite, MariaDB 등을 사용했습니다.



Q. NoSQL 중 여러가지가 있는데 왜 MongoDB를 썼어?

관심이 있지만, 사용하지 않았습니다 ㅠㅠ



Q. 쿼리가 어떻게 작동하는지 알아? (= SQL 튜닝 해봤어? )