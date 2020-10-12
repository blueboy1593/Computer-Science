# Python

Generator(제네레이터)는 제너레이터 함수가 호출될 때 반환되는 iterator(이터레이터)의 일종이다. 일반 함수와 비슷하게 생겼지만, yield 구문을 사용해 데이터를 원하는 시점에 반환하고 처리.

yield 문이 포함된 제네레이터 함수를 실행하면 객체가 반환됨.

List, Set, Dict 표현식은 iterable(이터러블)

MRO(method resolution order)

GIL = Global Interpreter Lock

쓰레드에서 사용되는 Lock을 인터프리터 레벨로 확장한 개념.

여러 스레드가 동시에 실행되는걸 방지한다. 어느 시점이든 하나의 Bytecode만이 실행되도록 강제함.

파이썬에도 garbage collection과 reference counting을 해서 할당된 메모리를 관리할 수 있다. 

Pypy는 파이썬으로 만들어진 파이썬 인터프리터이다. CPython보다 빠른 것을 확인 가능.

RPython은 PyPy 프로젝트 팀이 만든 일종의 인터프리터 제작 프레임워크

Timsort는 Python 내부의 sort

2.3버전부터 적용되었으며, merge sort와 insert sort가 병합된 형태의 안정정렬이다. merge sort 최악 시간 복잡도와 insert sort의 최고 시간 복잡도 보장한다. O(n) ~ O(n log n)의 시간 복잡도를 보장받음. 공간복잡도도 O(n)수준 안정정렬