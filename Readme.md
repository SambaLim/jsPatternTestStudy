# 자바스크립트 패턴과 테스트

래리스펜서, 세스 리처즈 지음 / 이일웅 옮김

# 1.1장

## SOLID

- Single Responsibility Principle(단일 책임의 원칙): 작성된 함수는 하나의 책임을 수행하는데 집중해야함
- Open/Closed Principle(개방 폐쇠의 원칙): 어떤 경우라도 실행 코드를 변경하지 말고, 어떻게든(상속 등의 방법으로) 재사용하고 확장하라
- Liskov Substitution Principle(리스코프 치환 법칙): 한 객체를 다른 객체에서 파생하더라도 그 기본 로직이 변경되어서는 안된다.
- Interface Segregation Principle(인터페이스 분리 원칙): 기능이 많은 인터페이스는 더 작게 응축시킨 조각으로 나누어야 한다는 발상
- Dependency Inversion Principle(의존성 역전 원칙): 상위 모듈은 하위 수준 모듈에 의존해서는 안되며 이 둘은 추상화에 의존해야 한다.

## DRY

- "모든 지식조각은 딱 한 번만 나와야한다."

# 1.2장

## 단위테스트

- 준비: 단위를 실행할 조건을 확실히 정하고, 의존성 및 함수 입력 데이터를 설정
- 실행: 단위를 실행하여 테스트
- 단언: 예상대로 단위가 작동하는지 확인

## TDD

- 적색
- 녹색
- 리팩터

# 2.2장

## 의존성 주입 프레임워크의 작동

1. 애플리케이션이 시작되자마자 주입가능한 모든 의존성을 확인하고 해당 의존성을 지칭하며 순서대로 DI컨테이너에 등록된다.
2. 객체가 필요하면 컨테이너에 요청한다.
3. 컨테이너는 일단 요청받은 객체와 그 의존성을 모두 재귀적으로 인스턴스화 한다. 그런 다음, 요건에 따라 필요한 객체에 각각 주입한다.