# HTML, CSS 메모

## 기초모듈

- div박스로 layout 만들 때, float정렬과 display : inline-block

inline-block로 해도 가능하지만, 글자를 썼을 때 글자의 baseline에 따라 박스가 발작하기 때문에 귀찮은 점이 많다.

- div 내부 컨텐츠 가운데 정렬

display: flex;

align-items: center;(세로정렬)

justify-content: center;(가로정렬)

### homework_1 확인

- selector문법

navbar > li : 직계자식만, navbar li : ~ 안에 있는 모든 자식, input[속성명=속성값] : ~ 속성을 가진 것만

- margin collapse 현상

div 박스 2개의 테두리가 겹칠경우 margin이 합쳐지게 됨. → 부모박스에 padding 살짝

- position 속성

좌표설정 가능(기준점 설정), 공중에 뜸! fixed 속성 쓰면 화면에 고정되는 컨텐츠 사용 가능 alsolute 속성(부모태그를 기준) + left, right 0, margin:auto 가운데정렬

- z-index

높을수록 위에 놓임

- box-sizing

그냥 width는 padding, border를 제외한 content영역을 의미, box-sizing : border-box; 를 추가해주면 됨.

- CSS 기본파일, nomalize

body의 margin:0; 이나 div의 box-sizing : border-box; 처럼 기본으로 설정 해두면 좋은 것들을 미리 css상단에 추가해두면 편하다.

또 브라우저마다 다르게 보이는 문제를 해결하기 위해 CSS normalize라는 문서를 사용할 수 있다.

- form, input

form에 action과 method로 어떤 경로로 어떤 요청(get, post)을 보낼지 정할 수 있다.

input type도 정말 다양하게 있고, name으로 서버에 전달. select, option태그로 선택박스 생성가능. 등등... 많으니 필요할 때 검색!

- float

float 해제시, 부모태그에서 가상요소(::after)를 생성하고

content:'';

display:block;

clear:both;

을 사용해주면 깔끔하게 가능.

- input과 label태그

label 태그에 for속성과 input의 id를 같게하면, label을 눌렀을 때 input을 누른 것과 같은 효과 (체크박스 등)

- table 레이아웃

table로 표를 만들수 있다. tr: 행, td: 열, thead, tbody, border-collapse: collapse 테두리 사이에 틈 없애기

- 사진 비율 유지하면서 컨테이너에 맞추기

object-fit: cover; 옵션 사용하면 가능

- nth-child(n)

~번째 자식 태그에 css적용하는 셀렉터

## 중급모듈

- 커스텀 폰트 사용법은 font-face

한글폰트는 용량이 커서 1~2개만 사용!, woff파일 사용하면 용량 줄어듦, 구글폰트 사용 가능

- 반응형 웹, 권장 breakpoint

media-quary 문법 사용

1200px / 992px / 768px / 576px ( ex. 1200 태블릿, 768 모바일)

- font awesome에서 아이콘 사용 가능

- 애니메이션 주기

1. 시작스타일, 최종스타일 만들기 2. 언제 최종스타일 되는지 (대부분 hover?, 아니면 JS사용) 3. transition 주기

- display: flex 공부...

- Bootstrap 사용하면 편하다

뼈대를 잡고, 세부사항은 직접 바꿔보기 (Utility class 사용 가능)

반응형 웹을 만들 때 매우 편리 (container, row, col - 조건식)

### 좋은 코드의 원칙

1. 나중에 수정/관리가 쉽다.

2. 확장성

## 고급모듈

- Pseudo-element

특정 html의 첫 글자, 첫 라인 꾸미기, 앞,뒤에 추가 등등 가능.

- Shadow DOM

HTML에 숨겨진 요소들. input에 css를 적용할 떄 사용 가능.

- 사이트 발행 방법

1. Github Pages 이용법 (도메인 주소는 상관없이 그냥 누구에게 보여줄 포트폴리오가 빠르게 필요할 때)

2. 일반 호스팅 이용법 (나의 도메인이 필요할 때)

## Sass 용도 및 문법

- scss파일을 css파일로 컴파일해서 사용. map파일은 크롬 개발자도구 디버깅용.

- 어려운 단어 기억, 변수 사용가능 ( $변수 = 어려운단어; ) > 수정과 관리가 쉬워짐, 사칙연산 가능, css로도 가능하지만 쬐끔 더 귀찮음

- scss, sass 차이? : 대괄호 있고 없고

- nesting 문법 : 

<img width="208" alt="스크린샷 2022-03-10 오후 6 28 23" src="https://user-images.githubusercontent.com/71241711/157632139-a5f08df3-5670-4b57-9293-615f229048ef.png">
이런 식으로 사용 가능.

- @extend 문법

중복되는 css 변수처럼 저장해서 사용. 

<img width="189" alt="스크린샷 2022-03-10 오후 6 34 21" src="https://user-images.githubusercontent.com/71241711/157633306-04509708-aee0-4076-bb6e-cda801f2fd21.png">


