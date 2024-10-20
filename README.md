### 1. Parser
기능 목표: 입력 문자열을 파싱하여 계산에 필요한 형태로 변환

- [ ] 빈 문자열 처리: 입력 문자열이 빈 문자열이거나 null일 경우 이를 처리하고 기본값을 반환하는 기능 구현
- [ ] 기본 구분자 파싱: 쉼표(,)와 콜론(:)을 기본 구분자로 지정하고, 이를 기준으로 숫자를 분리하는 기능 구현
- [ ] 커스텀 구분자 파싱: 커스텀 구분자가 존재할 경우 이를 추출하고 나머지 문자열을 분리하는 기능 구현
  - 문자열의 앞부분에 `//`와 `\n` 사이에 있는 구분자를 커스텀 구분자로 파싱

### 2. Calculator
기능 목표: 파싱된 숫자를 합산하여 결과 반환

- [ ] 숫자 합산 기능: 파싱된 숫자 리스트를 합산하는 기능 구현
  - 쉼표, 콜론, 커스텀 구분자로 분리된 숫자를 `Int` 타입으로 변환하고 합산
- [ ] 음수 입력 예외 처리: 음수가 포함된 경우 예외를 발생시키는 기능 구현 (`IllegalArgumentException`)
  - 음수 입력을 탐지하고, 적절한 에러 메시지와 함께 예외 발생

### 3. UI
기능 목표: 사용자와의 상호작용을 관리

- [ ] 입력값 요청: 사용자에게 덧셈할 문자열을 입력받는 기능 구현
  - `camp.nextstep.edu.missionutils.Console`의 `readLine()`을 사용해 입력받음
- [ ] 결과 출력: 계산된 결과를 사용자에게 출력하는 기능 구현
  - 계산 결과를 화면에 표시하는 기능 (`println`)
- [ ] 에러 메시지 출력: 예외가 발생했을 때 사용자에게 적절한 에러 메시지를 출력하고 종료하는 기능 구현

