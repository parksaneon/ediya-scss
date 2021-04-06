# EDIYA Sass Project

## 공통
- 모바일의 경우 .buttonBurger 요소에 클릭 이벤트 발생 시 .navigation 요소에 .is--active를 추가한다.

- 모바일 환경에서 .buttonClose 요소에 클릭 이벤트 발생 시 .navigation 요소에 .is--active를 제거한다.

- .buttonGoToTop를 클릭 시 페이지 상단으로 스크롤 시킨다.

## 로그인 및 회원가입 (signin.html / signup.html)
- 이메일, 패스워드, 패스워드 확인 입력 서식 (.input)에 입력 값이 유효할 경우 .is--valid, .is--invalid를 추가한다.
추가할 위치는 각각 .membership__email, .membership__password, .membership__passwordConfirm 이다.

- membership 관련 요소에 .is--valid나 .is--invalid가 추가될 때
해당 요소내 .iconNone 을 제거하고 대신 icon 클래스와 iconChecked 클래스 또는 icon 클래스와 iconWarning 클래스를 추가한다.
  - .is--valid 안에 .iconNone은 제거하고 .icon과 .iconChecked를 추가
  - .is--invalid 안에 .iconNone은 제거하고 .icon과 .iconWarning을 추가
- .is--invalid가 있을 경우 aria-live 속성을 사용하여 실시간으로 갱신된 정보를 읽을 수 있도록 한다. (이 부분은 aria-live 속성을 어디에 넣어야 할까요? input 요소일지 아니면 .is--invalid 클래스가 추가된 div 요소인지 헷갈려서 조언 구해요.)

- .membership__password와 .membership__passwordConfirm 영역의 경우 패스워드 보기 버튼을 클릭할 때마다 클래스를 토글 시킨다.
토글 시킬 클래스는 .buttonPassword 내 .iconInVisible을 .iconVisible로 .iconVisible을 .iconInVisible로 토글 시킨다.

- .buttonSignin(로그인 버튼), .linkSignup(회원가입 링크), .buttonSignup(가입하기 버튼) 등의 버튼 및 링크는 비활성화 상태의 경우 .is--disable를 추가하고 disable 속성도 함께 추가한다. 
이때 링크의 경우 disable 속성은 추가하지 않는다. (링크는 disable 속성을 줄 수 없기때문에 .is--disable 클래스를 추가하는 것만으로 해결되지 않을 것 같은데 cursor: not-allowed를 추가해 놔야 할까요? 이건 질문입니다.^^)

### 이디야 매장찾기(store.html)
- 매장찾기 관련 .tabUI__tab에 클릭 이벤트가 발생하면 해당 요소는 aria-selected="true"가 되고 나머지 요소는 aria-selected="false"가 되도록 한다.
- 선택된 탭 요소의 aria-controls 값을 제어하기 위해 해당 요소에 .is--selected를 추가시킨다.
(.storeName 또는 .storeAddress) 

### 뉴스(news.html)
- 뉴스 관련 .tabUI__tab에 클릭 이벤트가 발생하면 해당 요소는 aria-selected="true"가 되고 나머지 요소는 aria-selected="false"가 되도록 한다.

- 선택된 탭 요소의 aria-controls 값을 제어하기 위해 해당 요소에 .is--selected를 추가시킨다.
(.newsNotice 또는 .newsPress, .newsVideo, .newsAward) 

### 이디야 음료(beverage.html)
- 음료 버튼 (.beverage__button) 클릭 시 .beverage__detail 요소에 .is--active가 추가되도록 설정.
- 음료 상세 정보 다이얼로그 영역에서 닫기 버튼(.buttonClose) 클릭 시 .beverage__detail 요소에 .is--active를 제거한다.
