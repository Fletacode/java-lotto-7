# java-lotto-precourse

# 기능목록

---

## 로직 순서

1. 사용자에게 로또 구입 금액과 당첨번호, 보너스 번호를 입력받는다.

2. 구입한 금액만큼 로또를 발행한다.

3. 발행한 로또 수량 및 번호를 출력한다.

4. 당첨번호와 발행한 로또가 몇개가 일치한지 확인한다.

5. 당첨내역을 출력한다.

6. 수익률을 계산한후, 총 수익률을 출력한다.

---

## 기능 구현 사항

### 사용자 👤

#### 사용자는 유효한 로또 구입 금액을 입력할 수 있어야한다.

- [ ] 로또 구입 금액은 1000원 단위로 입력받으며, 숫자이다.
  - [ ] 사용자가 잘못된 입력을 하면,  `IllegalArgumentException` 을 발생시키고 애플리케이션을 종료한다.
    -  예외 처리 할 경우
    - [ ] 숫자가 아닐경우
    - [ ] 1000원 단위가 아닐경우
    
#### 사용자는 유효한 당첨번호를 입력할 수 있어야한다.

- [ ] 당첨번호는 , 단위로 구분한다.
- [ ] 사용자가 잘못된 입력을 하면, `IllegalArgumentException`을 발생시키고 애플리케이션을 종료한다.
    - 예외 처리 할 경우
    - [ ] 숫자가 아닌 값을 입력할 경우
    - [ ] , 구분자가 아닐경우
    - [ ] 1 미만, 45 초과인 수일 경우

#### 사용자는 유효한 보너스 번호 입력할 수 있어야한다.

- [ ] 보너스번호 하나를 입력받는다.
    - [ ] 사용자가 잘못된 입력을 하면, `IllegalArgumentException`을 발생시키고 애플리케이션을 종료한다.
    - 예외 처리 할 경우
        - [ ] 숫자가 아닌 값을 입력할 경우
        - [ ] 1 미만, 45 초과인 수일 경우

---

## 로또 🍀
- [ ] 구입한 금액만큼 로또를 발행해야한다.
    - [ ] 로또번호는 6개여야 한다.
    - [ ] 로또번호는 1~45여야 한다.
    - [ ] 구입한 금액 / 1000 == 개수이다.
- [ ] 당첨내역을 계산하여야한다.
  - [ ] 발행한 로또 번호와 당첨 번호, 보너스 번호가 몇개가 일치 한지 확인해야한다.
- [ ] 수익률을 계산해야한다.
  - [ ] 만약, 하나도 일치하지 않아 수익이 0이라면, 수익률을 0으로 계산한다.
  - [ ] 수익률은 소수점 둘째자리에서 반올림한다.

---

## 시스템 ⚙️
- [ ] 발행한 로또 수량 및 번호를 출력해야 한다.
    - [ ] 
    - [ ] ex) pobi : --
- [ ] 당첨내역을 출력해야한다.

- [ ] 수익률을 계산해야한다.
  -  [ ] 수익률은 소수점 둘째 자리에서 반올림한다.
- [ ] 에러 상황시 에러 문구를 출력해야한다.
  - ex) [ERROR] 로또 번호는 1부터 45사이의 숫자여야합니다. 