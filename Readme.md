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
