### 주어진 횟수동안 n대 자동차는 전진 또는 멈출 수 있다.
요구사항들

- 자동차이름 입력             #inputCar
  - (,)로 구분
  - 이름 5자 이하
- 시도 횟수 입력             #numberOfAttempts
- 조건 0~9무작위 값을 구하기   #randomValue
- 전진 출력칸                # moveCar
  - 자동차 이름 출력
  - 무작위 값이 4이상이면 전진 
- 우승자 알려줌              #winner
  - 시도 횟수 끝나고 - 제일 많은사람 알려줌
  - 공동 여러명이면 (,)이용해 구분
- 잘못된 값 입력시 : IllegalArgumentException 발생후 앱종료
- 게임 스타트               #gameRun


나눠야 할지 잘 모르겠는 것
- print문들
  - "경주할 자동차 이름을 입력하세요.(이름은 쉼표(,) 기준으로 구분)"
  - "시도할 횟수는 몇 회인가요?"
  - "실행 결과"
  - "최종 우승자"


변경 된 부분
- 조건 0~9무작위 값을 구하기   #randomValue
- 전진 출력칸                # moveCar
  - 자동차 이름 출력
    - 무작위 값이 4이상이면 전진 
이부분을    
- RacingCarGame 클래스 안에 다 넣음
  - 조건 0~9무작위 값을 구하기   #randomValue
  - 자동차 포지션 초기화 #initializeCarPosition
  - 무작위 값이 4이상이면 전진 #updateCarPosition
  - 이름, 전진 출력하기 #isplayCarPosition
  - 시도 횟수만큼 실행 #run

테스트 코드 작성해볼 것
- 5글자가 넘어가면 오류 발생 시키나
- 입력시 ','로 구분되게 입력이 되나
- 시도 횟수가 자연수로만 입력이 되나
- 0~9 값이 무작위로 잘 나오나
- 무작위 값이 4 이상일때만 전진하나
- 우승자가 여려명일때 ,로 구분되서 나오나