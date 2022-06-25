# ⚰ SpringStarBucks
Spring Boot를 이용한 커피 가게 구현하기 토이프로젝트

## Goals
1. `확장성`있는 설계 및 구현
2. `TDD`로 구현
3. 최대한 `클린코드`하게 구현

## 🎇 Tech
<img src="https://img.shields.io/badge/Java-003366?style=for-the-badge&logo=java&logoColor=white">
<img src="https://img.shields.io/badge/Spring Boot-6DB33F?style=for-the-badge&logo=spring boot&logoColor=white">
<img src="https://img.shields.io/badge/JPA-ED2762?style=for-the-badge&logo=Databricks&logoColor=white">
<img src="https://img.shields.io/badge/React-61DAFB?style=for-the-badge&logo=REACT&logoColor=white">

## Material
### 𝌭 도메인 모델

![Untitled](https://user-images.githubusercontent.com/68279162/175776120-d584800a-7f7e-401c-9737-0390a15e3db4.png)


- 손님은 커피점에서 사용할 돈을 충전할 수 있다.
    - (손님 ↔ 지갑)
- 손님은 메뉴판을 보고 직원에게 주문한다.
    - (손님 ↔ 메뉴판 / 손님 ↔ 점원)
- 직원은 손님의 주문 목록을 보고 커피를 제조하거나 디저트를 진열대에서 가져온다.
    - (직원 ↔ 커피, 콜드브루, 프라푸치노 / 직원 ↔ 디저트)
- 손님은 한번 주문을 하면 하나의 스탬프가 찍히게 된다. (손님 ↔ 스탬프)
    - 커피 하나에 스탬프 하나 찍힌다
    - 디저트는 스탬프 두개가 찍힌다
    - 스탬프가 10개 찍힌다면 아메리카노를 공짜로 먹을 수 있다.
    - 사용을 한다면 10개가 차감된다.
- 손님은 자신의 주문목록을 확인할 수 있다. (손님 ↔ 주문 목록)