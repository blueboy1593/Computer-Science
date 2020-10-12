# Javascript

싱글 스레드와 이벤트 루프란?

JavaScript Engine과 웹 브라우저에 화면을 그리는 Rendering Engine은 다른 것이다. 

구글에서 개발한 V8을 비롯해 대부분의 자바스크립트 엔진은 3가지 영역으로 나뉜다!

Call Stack / Task Queue / Heap

콜 스택은 단 하나의 호출 스택!!! 뭐 이렇게 표현할 수 있지.

bar라는 스택 프레임 foo 함수에서는 a + b라는 값.

event loop

자바스크립트 비동기 처리 과정은 RxJS Scheduler

쓰레드는 스택을 하나씩 갖고 있는 것 같다.

자바스크립트 처리 과정!! setTimeout promise1, 2, script end

Hoisting - 끌어올리기

호이스트란 변수의 정의가 범위에 따라 선언과 할당으로 분리되는 것을 의미한다. var x = 100;

함수 선언문 형태로 정의한 함수의 유효범위는 전체 코드의 맨 처음부터 시작한다. 선언이 실행 부분보다 뒤에 있더라도 자바스크립트 엔진이 함수 선언을 끌어올리는 것을 의미한다.

클로저(Closure)는 두 개의 함수로 만들어진 환경으로 이루어진 특별한 객체의 한 종류이다. 클로저 생성 시 범위에 있던 여러 지역 변수들이 포함된 context

bind / call / apply 메소드 등

화살표 함수는 function 표현방식보다 간결하게 함수를 표현 가능하지. 항상 익명이고, 자신의 this, arguments, super 그리고 new.target을 바인딩하지 않아

화살표 함수의 this는 상위 스코프 this와 동일한 값을 가진다 <=> 일반 함수에서는 아님.





