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

### UI UX

User Interface User experience

### CSR / SSR

Client Side Rendering

- 트래픽 감소
- 사용자 경험
- 검색 엔진...?

Server Side Rendering

- 검색 엔진 최적화
- 초기로딩 성능개선
- 프로젝트 복잡도
- 성능 악화 가능성

### SPA(Single Page Application)

최초 한 번 페이지 전체를 로딩한 뒤, 데이터만 변경하여 사용할 수 있는 애플리케이션

기본적으로 페이지 로드가 없음

새로고침을 너모 많이 하면 안됨

### Vue.js 그리고 React

개발 CLI

vue-cli / create-react-app

Vue.js는 css파일이 기본적으로 없고, style을 컴포넌트 파일 안에서 정의합니다.

React는 css 파일이 존재하며, 해당 파일을 통해 style을 적용합니다.

### 데이터 변이

Vue.js는 반드시 데이터 객체를 생성한 이후 data를 업데이트 할 수 있음

React는 state 객체를 만들고, 업데이트에 조금 더 작업이 필요

### PWA(Progressive Web App)

웹의 장점과 앱의 장점을 결합한 환경

### 서비스 작업자(Service Worker) API

웹앱의 중요한 부분을 캐싱하여 사용자가 다음에 열 때 빠르게 로딩할 수 있도록 도와줌

### Vue.js의 라이프사이클

은 크게 4가지로 나누어진다.

1. Creation
2. Mounting
3. Updating
4. Destruction

beforeCreate

가장 먼저 실행되는 훅

created

데이터, 이벤트가 활성화되어 접근이 가능함

하지만 아직 템플릿과 virtual DOM은 마운트 및 렌더링 되지 않은 상태임

2) Mounting

초기 렌더링 직전 컴포넌트에 직접 접근이 가능

컴포넌트 초기 세팅 데이터들은 created에서 사용하는 것이 나음

3) Updating

beforeUpdate

updated

컴포넌트의 데이터가 변하여 다시 렌더링된 이후에 실행됨

업데이트가 완료된 상태이므로, DOM 종속적인 연산이 가능

4) Destruction

해체 단계

beforeDestroy

destroyed

### computed

는 템플릿에 데이터를 바인딩 할 수 있습니다.

```vue
<div id="example">
  <p>원본 메시지: "{{ message }}"</p>
  <p>역순으로 표시한 메시지: "{{ reversedMessage }}"</p>
</div>
 
<script>
    new Vue({
      el: '#example',
      data: {
        message: '안녕하세요'
      },
      computed: {
        // 계산된 getter
        reversedMessage: function () {
        // `this` 는 vm 인스턴스를 가리킵니다.
        return this.message.split('').reverse().join('')
        }
      }
     })
</script>
```

이런 코드가 있다고 가정할 때, message의 값이 바뀌면, reversedMessage의 값도 따라 바뀐다.

Computed는 선언형, watch는 명령형 프로그래밍 방식이라고 합니다.







