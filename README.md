# Market-karly
> 웹 접근성과 성능에 집중한 웹 사이트

## 구현 기능
### main
- 사이트가 열리면 팝업창이 뜨고 닫기를 누르면 닫힌다.
- main_banner의 슬라이드가 자동으로 움직이고 마우스와 키보드로 통제 할 수 있다.
- 상품 추천에서 장바구니 아이콘을 클릭하면 장바구니 모달창이 뜬다.
- 상품을 클릭하면 최근 본 항목이 뜨고 해당 상품이 담긴다.

### login
- 사용자가 id 비밀번호를 입력한다.
- data.json에 해당하는 id와 비밀번호가 일치 할 경우 localstorage에 key로 unique ID, value로 아이디를 저장한다.

### register
- 사용자가 본인에 대한 정보를 기입한다.
- 필수 입력 조건이 성립되지 않은 경우 가입하기 버튼이 비활성화 처리 된다.

### cart
- 체크 버튼이 아닌 텍스트를 눌러도 체크가 되도록 한다.
- 전체 체크 선택을 하면 상품리스트가 전체 체크되고, 개별 선택을 하면 전체 체크가 풀리고 해당 상품만 클릭이 된다.
- 수량 증감버튼을 눌렀을 때에 맞춰 상품 수량이 증가하거나 감소하고, 1이하로는 떨어지지 않게 해준다. 
- 수량 증감 버튼을 누를시 아이콘이 클릭되고 있다는 것을 보여주기위해 아이콘 색을 다르게해 활성화 시켜준다.
- 수량 증감버튼을 누르면 상품의 가격도 같이 증감한다.

### product list
- 카테고리 메뉴를 아코디언 메뉴로 구성해 클릭했을 때 접었다 펼치는 기능을 넣어준다.
- 카테고리 내 목록을 선택했을 때 선택되고 있다는 것을 직관적으로 알려주기 위해서 hover시 폰트 색상을 변경한다.
- 아이콘이 아닌 타이틀을 눌러도 체크 아이콘이 활성화 되도록 만들어준다.
- 카테고리 메뉴를 선택했을 때 초기화 버튼을 활성화시킨다.
- 목록을 선택 후 초기화 버튼을 누르면 카테고리 목록을 지워주고 초기화 버튼도 비활성화 시킨다.

### detail
- 사용자가 상품 수량을 선택하면, 그에 따라 총 상품금액이 변동되며, 총 금액은 세자리마다 콤마가 찍힌다.
- 사용자가 '장바구니 담기'버튼을 클릭하면 헤더의 장바구니 아이콘 아래쪽에 장바구니에 상품을 담았다는 말풍선이 뜬다.
- 네비게이션바가 스크롤을 내려서 화면상에 보이지 않게 되는 경우를 대비해, 네비게이션바를 상단에 고정한다.
- 네비게이션바에서 원하는 영역을 선택하면 해당영역으로 화면초점이 이동한다.
- 상품후기와 문의의 공지를 클릭하면 접힌 공지내용이 나온다. 
- 후기 작성하기 버튼과 문의하기 버튼을 클릭하면 작성할 수 있는 팝업이 뜬다.
- 각 게시판 아래 화살표 버튼을 클릭하면 다음 슬라이드로 이동한다. 

---
## 성능 
- 이미지 최적화를 위해 아이콘을 제외한 이미지는 webP형식으로 통일한다.

---
## 개발 환경
### 클라이언트만 개발하는 경우
- 본 저장소를 클론 받은 후, 루트 디렉터리에서 `npm install`, `npm start`을 해서 구동한다.
