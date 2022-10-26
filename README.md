# 로또

## 진행 방법

* 로또 요구사항을 파악한다.
* 요구사항에 대한 구현을 완료한 후 자신의 github 아이디에 해당하는 브랜치에 Pull Request(이하 PR)를 통해 코드 리뷰 요청을 한다.
* 코드 리뷰 피드백에 대한 개선 작업을 하고 다시 PUSH한다.
* 모든 피드백을 완료하면 다음 단계를 도전하고 앞의 과정을 반복한다.

## 온라인 코드 리뷰 과정

* [텍스트와 이미지로 살펴보는 온라인 코드 리뷰 과정](https://github.com/next-step/nextstep-docs/tree/master/codereview)

## 🚀 1단계 - 학습 테스트 실습

### 요구사항

- String 클래스에 대한 학습 테스트
    - [x] "1,2"을 ,로 split 했을 때 1과 2로 분리된다.
    - [x] "1"을 ,로 split 했을 때 1만을 포함하는 배열 반환된다.
    - [x] "(1,2)" 값이 주어졌을 때 String의 substring() 메소드를 활용해 ()을 제거하고 "1,2" 를 반환할 수 있다.
    - [x] "abc" 값이 주어졌을 때 String의 charAt() 메소드를 활용해 특정 위치의 문자를 가져올 수 잇다.
    - [x] String의 charAt() 메소드를 활용해 특정 위치의 문자를 가져올 때 위치 값을 벗어나면 StringIndexOutOfBoundsException을 발생시킨다.
- Set Collection에 대한 학습 테스트
    - [x] Set의 size() 메소드를 활용해 Set의 크기를 확인한다.
    - [x] Set의 contains() 메소드를 활용해 값이 존재하는지 확인한다.
    - [x] Set의 contains() 메소드를 활용해 값이 존재하지 않음을 확인한다.

---

## 🚀 2단계 - 문자열 덧셈 계산기

### 요구사항

- [x] 빈 문자열 또는 null 값을 입력할 경우 0을 반환해야 한다.
- [x] 숫자 하나를 문자열로 입력할 경우 해당 숫자를 반환한다.
- [x] 숫자 두개를 컴마(,) 구분자로 입력할 경우 두 숫자의 합을 반환한다.
- [x] 구분자를 컴마(,) 이외에 콜론(:)을 사용할 수 있다.
- [x] “//”와 “\n” 문자 사이에 커스텀 구분자를 지정할 수 있다.
- [x] 숫자 이외의 값 또는 음수를 전달할 경우 RuntimeException 예외가 발생해야 한다.

---
## 🚀 3단계 - 로또(자동)

### 요구사항

- 도메인
  - 숫자
    - [ ] 1 ~ 45 사이의 숫자만 가능하다.
  - 금액
     - [ ] 로또 한장의 가격은 1000원이다.
     - [ ] 구매 금액으로 1000원 이상의 숫자를 입력해야 한다.
     - [ ] 구매가능한 로또 수를 계산한다.
  - 로또
     - [ ] 구맥 가능한 만큰 자동으로 로또를 구매한다.
  - 당첨번호
     - [ ] 당첨 번호를 가지고 있다.
     - [ ] 번호를 비교해서 당첨 여부를 비교한다.
  - 순위
     - [ ] 5개로 구분된다.
     - [ ] 일치 갯수를 통해서 순위 타입을 리턴한다.
  - 당첨 통계
     - [ ] 당첨 내역을 가지고 있다.
     - [ ] 수익률을 계산한다.
- 입출력
  - 입력
    - [ ] 구매금액
    - [ ] 당첨번호
  - 출력
    - [ ] 구매 가능한 로또 수
    - [ ] 구매한 로또의 번호
    - [ ] 당첨 통계
    - [ ] 수익률
