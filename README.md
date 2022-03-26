# 키친포스

## 요구 사항

### 상품

- 상품을 등록할 수 있다.
- 상품의 가격이 올바르지 않으면 등록할 수 없다.
    - 상품의 가격은 0원 이상이어야 한다.
- 상품의 이름이 올바르지 않으면 등록할 수 없다.
    - 상품의 이름에는 비속어가 포함될 수 없다.
- 상품의 가격을 변경할 수 있다.
- 상품의 가격이 올바르지 않으면 변경할 수 없다.
    - 상품의 가격은 0원 이상이어야 한다.
- 상품의 가격이 변경될 때 메뉴의 가격이 메뉴에 속한 상품 금액의 합보다 크면 메뉴가 숨겨진다.
- 상품의 목록을 조회할 수 있다.

### 메뉴 그룹

- 메뉴 그룹을 등록할 수 있다.
- 메뉴 그룹의 이름이 올바르지 않으면 등록할 수 없다.
    - 메뉴 그룹의 이름은 비워 둘 수 없다.
- 메뉴 그룹의 목록을 조회할 수 있다.

### 메뉴

- 1 개 이상의 등록된 상품으로 메뉴를 등록할 수 있다.
- 상품이 없으면 등록할 수 없다.
- 메뉴에 속한 상품의 수량은 0 이상이어야 한다.
- 메뉴의 가격이 올바르지 않으면 등록할 수 없다.
    - 메뉴의 가격은 0원 이상이어야 한다.
- 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
- 메뉴는 특정 메뉴 그룹에 속해야 한다.
- 메뉴의 이름이 올바르지 않으면 등록할 수 없다.
    - 메뉴의 이름에는 비속어가 포함될 수 없다.
- 메뉴의 가격을 변경할 수 있다.
- 메뉴의 가격이 올바르지 않으면 변경할 수 없다.
    - 메뉴의 가격은 0원 이상이어야 한다.
- 메뉴에 속한 상품 금액의 합은 메뉴의 가격보다 크거나 같아야 한다.
- 메뉴를 노출할 수 있다.
- 메뉴의 가격이 메뉴에 속한 상품 금액의 합보다 높을 경우 메뉴를 노출할 수 없다.
- 메뉴를 숨길 수 있다.
- 메뉴의 목록을 조회할 수 있다.

### 주문 테이블

- 주문 테이블을 등록할 수 있다.
- 주문 테이블의 이름이 올바르지 않으면 등록할 수 없다.
    - 주문 테이블의 이름은 비워 둘 수 없다.
- 빈 테이블을 해지할 수 있다.
- 빈 테이블로 설정할 수 있다.
- 완료되지 않은 주문이 있는 주문 테이블은 빈 테이블로 설정할 수 없다.
- 방문한 손님 수를 변경할 수 있다.
- 방문한 손님 수가 올바르지 않으면 변경할 수 없다.
    - 방문한 손님 수는 0 이상이어야 한다.
- 빈 테이블은 방문한 손님 수를 변경할 수 없다.
- 주문 테이블의 목록을 조회할 수 있다.

### 주문

- 1개 이상의 등록된 메뉴로 배달 주문을 등록할 수 있다.
- 1개 이상의 등록된 메뉴로 포장 주문을 등록할 수 있다.
- 1개 이상의 등록된 메뉴로 매장 주문을 등록할 수 있다.
- 주문 유형이 올바르지 않으면 등록할 수 없다.
- 메뉴가 없으면 등록할 수 없다.
- 매장 주문은 주문 항목의 수량이 0 미만일 수 있다.
- 매장 주문을 제외한 주문의 경우 주문 항목의 수량은 0 이상이어야 한다.
- 배달 주소가 올바르지 않으면 배달 주문을 등록할 수 없다.
    - 배달 주소는 비워 둘 수 없다.
- 빈 테이블에는 매장 주문을 등록할 수 없다.
- 숨겨진 메뉴는 주문할 수 없다.
- 주문한 메뉴의 가격은 실제 메뉴 가격과 일치해야 한다.
- 주문을 접수한다.
- 접수 대기 중인 주문만 접수할 수 있다.
- 배달 주문을 접수되면 배달 대행사를 호출한다.
- 주문을 서빙한다.
- 접수된 주문만 서빙할 수 있다.
- 주문을 배달한다.
- 배달 주문만 배달할 수 있다.
- 서빙된 주문만 배달할 수 있다.
- 주문을 배달 완료한다.
- 배달 중인 주문만 배달 완료할 수 있다.
- 주문을 완료한다.
- 배달 주문의 경우 배달 완료된 주문만 완료할 수 있다.
- 포장 및 매장 주문의 경우 서빙된 주문만 완료할 수 있다.
- 주문 테이블의 모든 매장 주문이 완료되면 빈 테이블로 설정한다.
- 완료되지 않은 매장 주문이 있는 주문 테이블은 빈 테이블로 설정하지 않는다.
- 주문 목록을 조회할 수 있다.

## 용어 사전

| 한글명 | 영문명 | 설명 |
| --- | --- | --- |
| 포스 | POS | 판매시점 정보관리를 담당하는 기기 |
| 상품 | PRODUCT | 돈으로 거래될 수 있는 제품. 가격과 이름이 포함된다. |
| 메뉴 | MENU | 손님에게 제공하기 위한 음식의 목록과 가격이 포함된다. |
| 메뉴 그룹 | MENU GROUP | 메뉴를 묶은 메뉴의 상위카테고리이다. |
| 메뉴 상품 | MENU PRODUCT | 메뉴에 담기는 상품과 갯수 |
| 숨김 | HIDE | 메뉴를 손님이 확인할 수 없는 상태 |
| 공개 여부 | DISPLAY | 메뉴를 손님에게 보여줄지 여부 |
| 주문 | ORDER | 손님이 식사를 하기위해 메뉴를 지정하는 행위 |
| 주문 라인 아이템 | ORDER LINE ITEM | 주문에 담기는 세부 주문 정보 |
| 주문 상태 | ORDER STATUS | 주문이 시작되면 실행되는 단계 |
| 대기 | WAITING | 주문이 실행되면 가게의 승인을 기다리는 주문상태 |
| 승인 | ACCEPTED | 가게의 주문 승인이 된 주문상태 |
| 조리 | SERVED | 음식을 만드는 주문상태 |
| 배달중 | DELIVERING | 조리된 음식을 손님에게 배달중인 주문상태 |
| 배달완료 | DELIVERED | 조리된 음식을 손님에게 배달완료한 주문상태 |
| 주문완료 | COMPLETED | 주문이 종료된 준문상태 |
| 주문형태 | ORDER TYPE | 주문을 전달받는 형태 |
| 배달 | DELIVERY | 손님이 식사를 주문하여 음식 전달받는 주문형태 |
| 포장 | TAKEOUT | 손님이 식사를 주문하여 음식을 직접 가져가는 주문형태 |
| 식당식사 | EAT IN | 손님이 식사를 주문하여 식당에서 식사를 하는 주문형태 |
| 배달주소 | DELIVERY ADDRESS | 손님의 주문형태가 배달일 때 주문을 전달할 장소 |
| 키친 라이더 클라이언트 | KITCHEN RIDERS CLIENT | 배달요청을 하기 위해 사용되는 클라이언트 |
| 앉음 | SIT | 손님이 테이블을 사용하는 테이블상태 |
| 해제 | CLEAR | 손님이 테이블을 사용하지 않는 테이블상태 |
| 테이블 | TABLE | 손님이 식당에서 식사를 하면 식사를 하게되는 곳 |

## 모델링

### PRODUCT(상품)
- 속성
  - `PRODUCT`는 `PROUDCT`를 구별할 수 있는 `PROUDCT ID`를 가진다.
  - `PRODUCT`은 `NAME(이름)`을 가진다.
  - `PRODUCT`은 0 이상 `PRICE(가격)`을 가진다.
- 기능
  - `PRODUCT`을 등록할 수 있다.
    - `PRICE(가격)`는 0보다 커야한다.
    - `NAME(이름)`이 있어야한다.
    - `NAME(이름)`에 `PROFANITY(비속어)`는 사용할 수 없다.
  - `PRODUCT`의 `PRICE(가격)`를 변경할 수 있다.
    - `PRICE(가격)`는 0보다 커야한다.
    - `MENU(메뉴)`의 `PRICE(가격)`이 `MENU PRODUCT(메뉴상품)`의 합보다 크면 메뉴는 `HIDE(숨김)`이 된다.
  - `PRODUCT` 목록을 조회할 수 있다.

### MENU(메뉴)

- 속성
  - `MENU`는 `MENU`를 구별할 수 있는 `메뉴 ID`를 가진다.
  - `MENU`는 `NAME(이름)`을 가진다.
  - `MENU`는 0 이상 `PRICE(가격)`을 가진다.
  - `MENU`는 `MENU GROUP(메뉴그룹)`에 포함된다.
    - `MENU GROUP(메뉴 그룹)`을 구별할 수 있는 `MENU GROUP ID`를 가진다.
  - `MENU`는 `DISPLAY(공개 여부)` 속성을 가진다.
  - `MENU`는 `MENU PRODUCT(메뉴상품)`을 한 개 이상 가진다.

- 기능
  - `MENU`를 등록할 수 있다.
    - `MENU`의 `PRICE(가격)`은 `MENU`가 가진 `MENU PRODUCT(메뉴상품)`의 합보다 클 수 없다.
    - `MENU`의 `PRICE(가격)`은 0 이상이어야한다.
    - `MENU`의 `NAME(이름)`에 `PROFANITY(비속어)`는 사용할 수 없다.
    - `NAME(이름)`이 있어야한다.
    - `MENU PRODDUCT(메뉴 상품)`의 `QUANTITY(수량)`이 0 이상이어야한다.
    - `MENU GROUP(메뉴 그룹)`에 포함되어 있어야한다.
- `MENU`의 가격을 변경할 수 있다.
  - `MENU`의 `PRICE(가격)`은 `MENU`가 가진 `MENU PRODUCT(메뉴상품)`의 합보다 클 수 없다.
  - `MENU`의 `PRICE(가격)`은 0 이상이어야한다.
- `MENU`의 `DISPLAY(공개 여부)` 상태를 활성화 할 수 있다.
  - `MEMU`의 `PRICE(가격)`이 `MENU PRODUCT(메뉴상품)`의 합보다 크면 활성화 할 수 없다.
- `MENU`의 `DISPLAY` 상태를 `HIDE(숨김)` 할 수 있다.
- `MENU`의 목록을 조회 할 수 있다.

### MENU GROUP(메뉴 그룹)
- 속성
  - `MENU GROUP`은 `MENU GROUP`을 구별할 수 있는 `MENU GROUP ID`를 가진다.
  - `NAME(이름)`이 있어야한다.
- `MENU GROUP`을 등록 할 수 있다.
  - `NAME(이름)`이 있어야한다.
- `MENU GROUP` 목록을 조회 할 수 있다.

### 주문

- `주문`은 `주문`을 구별할 수 있는 `주문 ID`를 가진다.
- `주문`은 `주문 타입`을 가진다.
- `주문`은 `주문 상태`를 가진다.
- `주문`은 `주문 시간`를 가진다.
- `주문`은 한 개 이상의 `주문 라인 아이템`을 가진다.
- `주문`을 `생성`할 수 있다.
  - `주문`이 `식당식사`이면, `생성`시 `주문 테이블`이 있어야한다.
  - `주문`이 `식당식사`이면, `생성`시 `수량`이 0보다 커야한다.
- `주문`을 `수락`할 수 있다.
  - `주문상태`가 `주문대기` 여야한다.
- `주문`을 `조리`할 수 있다.
  - `주문상태`가 `수락`상태여야한다.
- `주문`을 `배달시작`할 수 있다.
  - `주문`이 `배달`이어야한다.
  - `주문 상태가`이 `조리`이어야한다.
- `주문`이 `배달`이면, `배달 시작`시 `주문 상태`가 `조리`면 안된다.
- `주문`을 `배달 완료` 할 수 있다.
  - `주문`이 `배달`이면, `배달 완료`시 `주문 상태`가 `배달중`이면 안된다.
- `주문`을 `주문 완료` 할 수 있다.
  - `주문`이 `식당식사`이면, `주문완료`시 `주문 상태`가 `조리`면 안된다.
  - `주문`이 `식당식사`이면, `주문완료`시 `주문 테이블`를 `해제`상태로 설정한다.
  - `주문`이 `포장`이면, `주문완료`시 `주문 상태`가 `조리`면 안된다.
  - `주문`이 `배달`이면, `주문완료`시 `주문 상태`가 `배달완료`여야한다.

### 주문 테이블

- `주문 테이블`는 `주문 테이블`을 구별할 수 있는 `주문테이블 ID`를 가진다.
- `주문 테이블`는 `이름`을 가진다.
- `주문 테이블`는 `손님수`을 가진다.
- `주문 테이블`는 `비어있는` 상태를 가진다.
- `주문 테이블`을 `생성`할 수 있다.
  - 최초 생성시 `손님수`는 0명이다.
  - 최초 생성시 `비어있다`
- `주문 테이블`을 `앉을` 수 있다.
  - `주문 테이블`은 `비어있지` 않다.
- `주문 테이블`을 `해제`할 수 있다.
  - `주문 상태`가 `주문 완료`여야한다.
  - `해제`시 `손님수`는 0이다.
  - `해제`시 `주문테이블`은 `비어있다`
- `주문테이블`의 `손님 수`를 변경할 수 있다
  - 변경할 `손님수`는 0보다 커야한다.
  - `비어있음` 상태가 되면 안된다
- `주문 테이블` 목록을 조회할 수 있다.
