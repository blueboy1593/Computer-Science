# Web

브라우저의 동작 방법!!! Web의 기본적인 과정이다.

www.naver.com을 입력했을 때, 어떤 과정을 거쳐서 네이버 페이지가 보이는지 알아보자.

브라우저의 주요 기능

사용자가 선택한 자원을 서버에 요청, 브라우저에 표시

자원은 html 문서, pdf, image 등 다양한 형태이다

자원의 주소는 URI에 의해 정해짐

브라우저는 html과 css 명세에 따라서 html 파일을 해석해서 표시한다.

W3C(World wide web Consortium)에서 정해진다.

사용자 인터페이스 -> 브라우저 엔진 -> 렌더링 엔진 -> (통신, 자바스크립트 해석기, UI 백엔드) -> 브라우저 엔진에서 자료저장소로

사용자 인터페이스 : 주소 표시줄, 이전/다음 버튼, 북마크 등 사용자가 활용하는 서비스들

브라우저 엔진 : 사용자 인터페이스와 렌더링 엔진 사이의 동작 제어

렌더링 엔진 : 요청한 콘텐츠 표시(html요청 -> html, css 파싱해서 표시)

통신 : http 요청과 같은 네트워크 호출에 사용

UI 백엔드

렌더링 엔진 종류

크롬, 사파리 : 웹킷(Webkit) 엔진 사용

파이어폭스 : 게코(Gecko) 엔진 사용

DOM 이란?

Document Object Model(문서 객체 모델)

파싱(parsing) : 브라우저가 코드를 이해하고 사용할 수 있는 구조로 변환하는 것

파서 생성기

### HTTP Status Code

100 : 정보 확인

200 : 통신 성공

200은 Get 성공!

201은 Post 성공!!

202는 요청 접수 O

204는 요청 성공, no content

300번대: 리다이렉트

300 Multiple Choice 요청 URI에 여러 리소스가 존재

301 Move Permanently 요청 URI가 새 위치로 옮겨감

304 Not Modified 요청 URI의 내용이 변경 X

400번대 : 클라이언트 오류

400은 Bad Request : API에서 정의되지 않은 요청이 들어옴

401은 Unauthorized : 인증 오류

403은 Forbidden 권한 밖의 접근 시도

404는 Not Found 요청 URI에 대한 리소스 존재 X

405는 Method Not Allowed API에서 정의되지 않은 메소드 호출

500번대는 서버 오류

500은 Internal Server Error 서버 내부 오류

502는 Bad Gateway 게이트웨이 오류

503은 Service Unavailable 서비스 이용 불가

504는 Gateway Timeout 게이트웨이 시간 초과

### REST API

Representational State Transfer 기본

**Idempotent** : 한번 수행하냐? 여러번 수행했을 때 결과가 같은가?

Resource

http://myweb/users와 같은 URI

Message : JSON과 XML같은 형태와 포멧이 있음!!!

Statelessness

HTTP session과 같은 컨텍스트 저장소에 상태 정보 저장 안함

request만 message로 처리하면 되고 구현이 단순해짐

Static Pages 바뀌지 않는 페이지

Dynamic Pages

인자에 따라 바뀌는 페이지

개념에 있어서 하드웨어와 소프트웨어로 구분!

하드웨어 : Web 서버가 설치되어 있는 컴퓨터

소프트웨어 : 웹 브라우저 클라이언트로부터 HTTP 요청을 받고, 정적인 컨텐츠(html, css 등)을 제공하는 컴퓨터 프로그램

### WAS

Web Application Server의 약자

HTTP를 통해 애플리케이션을 수행해주는 미들웨어

웹 컨테이너 혹은 서블릿 컨테이너

Open Authentification

서비스 제공자

소비자 비밀번호

요청 토큰 / 접근 토큰

Access Token / Refresh Token

소비자가 서비스 제공자에게 요청토큰을 요청한다.

### JWT (JSON Web Token)

.을 구분자로 3가지의 문자열로 구성되어 있다.

aaaa.bbbbb.ccccc 구조로 앞에서부터 헤더(header), 내용(payload), 서명(signature)으로 구성된다.

typ : 토큰의 타입을 지정합니다.

alg: 해싱 알고리즘을 지정합니다.

HMAC, SHA256, RSA가 사용되고, signature

iss : 토큰 발급자

iat : 토큰이 발급된 시간 - issued at / 토큰의 age가 얼마나 되었는지 판단 가능ㄴ

jti : JWT의 고유 식별자로서, 주로 중복적인 처리를 방지하기 위해 사용. 일회용 토큰에 사용하면 유용하다.

서명 - singature

해쉬를 base64 형태로 나타낸다!!!

### API Key







