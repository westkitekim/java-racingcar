# 📍[미션1] 자동차 경주 게임
<!-- Orginal
## 진행 방법
* 자동차 경주 게임 요구사항을 파악한다.
* 요구사항에 대한 구현을 완료한 후 자신의 github 아이디에 해당하는 브랜치에 Pull Request(이하 PR)를 통해 코드 리뷰 요청을 한다.
* 코드 리뷰 피드백에 대한 개선 작업을 하고 다시 PUSH한다.
* 모든 피드백을 완료하면 다음 단계를 도전하고 앞의 과정을 반복한다.

## 온라인 코드 리뷰 과정
* [텍스트와 이미지로 살펴보는 온라인 코드 리뷰 과정](https://github.com/next-step/nextstep-docs/tree/master/codereview)
-->

##  💡 3단계 - 자동차 경주
### 기능 요구사항
1. 초간단 자동차 경주 게임을 구현한다.
2. 주어진 횟수 동안 n대의 자동차는 전진 또는 멈출 수 있다.
   - [x] 입력받은 n대의 자동차가 전진한다.
3. 사용자는 몇 대의 자동차로 몇 번의 이동을 할 것인지를 입력할 수 있어야 한다.
   - [x] 자동차 대수(n)를 입력받는다.
      - [x] 자동차 대수가 담긴 리스트를 생성한다.
      - [ ] **(검증)** 자동차 대수가 0 이하인 경우 예외를 던진다. (_**UI 단위테스트 제외**_)
      - [ ] **(검증)** 자동차 대수가 정수가 아닌 경우 예외를 던진다. (_**UI 단위테스트 제외**_)
   - [x] 자동차 이동 횟수를 입력받는다
4. 전진하는 조건은 0에서 9 사이에서 random 값을 구한 후 random 값이 4이상일 경우이다.
   - [x] 0~9 사이의 random 값을 구한다.
   - [x] random 값이 0 이상 3 이하인 경우 전진하지 않는다.(정지)
   - [x] random 값이 4 이상 9 이하인 경우 전진한다.
5. 자동차의 상태를 화면에 출력한다. 어느 시점에 출력할 것인지에 대한 제약은 없다.
   - [x] 자동차 경주 과정을 출력한다.

---
##  💡 4단계 - 자동차 경주(우승자)
### 기능 요구사항
1. 각 자동차에 이름을 부여할 수 있다. 자동차 이름은 5자를 초과할 수 없다.
2. 전진하는 자동차를 출력할 때 자동차 이름을 같이 출력한다.
3. 자동차 이름은 쉼표(,)를 기준으로 구분한다.
4. 자동차 경주 게임을 완료한 후 누가 우승했는지를 알려준다. 우승자는 한명 이상일 수 있다.


#### Validation 
- [x] 자동차 이름이 5자를 초과하면 예외를 던진다.
- [x] 자동차 이름이 null이거나 빈 문자열이면 에러를 던진다.  


#### Domain
- [ ] 자동차의 이름을 쉼표(,)를 기준으로 구분한다.
- [ ] 사용자가 입력한 이름의 숫자 만큼 자동차 대수를 생성한다.
- [ ] 자동차의 이름과 위치 정보를 가지는 Car 객체를 수정하여 구현한다.  


#### View
- [ ] 입력부 초기 메세지 수정 ("경주할 자동차 이름을 입력하세요(이름은 쉼표(,)를 기준으로 구분).")
- [ ] 출력시 자동차의 이름과 위치, 우승자들을 함께 출력한다.  
