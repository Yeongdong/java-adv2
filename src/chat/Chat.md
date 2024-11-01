# 채팅 프로그램 정리

* Null Object Pattern
    * null을 객체처럼 처리하는 방법
    * null 대신 사용할 수 있는 특별한 객체를 만들어, null로 인해 발생할 수 있는 예외 상황을 방지하고 코드의 간결성을 높이는데 목적이 있다.
    * 이 패턴을 사용하면 null 값 대신 특정 동작을 하는 객체를 반환하게 되어, 클라이언트 코드에서 null 체크를 할 필요가 없어진다.
    * 코드에서 불필요한 조건문을 줄이고 객체의 기본 동작을 정의하는데 유용하다.
* Command Pattern
    * Command 인터페이스와 그 구현체들을 사용한 것
    * 요청을 독립적인 객체로 변환해서 처리
* 분리: 작업을 호출하는 객체와 작업을 수행하는 객체를 분리한다.
* 확장성: 기존 코드를 변경하지 않고 새로운 명령을 추가할 수 있다.
* 장점
    * 새로운 커맨드를 쉽게 추가할 수 있다.
    * 작업을 호출하는 객체와 작업을 수행하는 객체가 분리되어 있다. 이전 코드에서는 작업을 호출하는 if 문이 각 작업마다 등장했는데, 커맨트 패턴에서는 이런 부분을 하나로 모아서 처리할 수 있다.
    * 각각의 기능이 명확히 분리된다.
* 단점
    * 복잡성 증가
        * 간단한 작업을 수행하는 겨웅에서 여러 클래스를 생성해야 한다.