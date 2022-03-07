<div>
  <h1> HTML, CSS 메모 </h1>
  <ul>
    <h2>기초모듈</h2>
    <li>div박스로 layout 만들 때, float정렬과 display : inline-block</li>
    <p> inline-block로 해도 가능하지만, 글자를 썼을 때 글자의 baseline에 따라 박스가 발작하기 때문에 귀찮은 점이 많다. </p>
    <li>div 내부 컨텐츠 가운데 정렬</li>
    <p>  display: flex;<br>
      align-items: center;(세로정렬)<br>
      justify-content: center;(가로정렬)<br>
      homework_1 확인 <p>
  <li> selector문법</li>
  <p> navbar > li : 직계자식만, navbar li : ~ 안에 있는 모든 자식, input[속성명=속성값] : ~ 속성을 가진 것만</p>
  <li> margin collapse 현상 </li>
  <p> div 박스 2개의 테두리가 겹칠경우 margin이 합쳐지게 됨. → 부모박스에 padding 살짝 </p>
  <li> position 속성 </li>
  <p> 좌표설정 가능(기준점 설정), 공중에 뜸! <br>fixed 속성 쓰면 화면에 고정되는 컨텐츠 사용 가능<br> alsolute 속성(부모태그를 기준) + left, right 0, margin:auto 가운데정렬</p>
  <li> z-index </li>
  <p> 높을수록 위에 놓임 </p>
  <li> box-sizing </li>
  <p> 그냥 width는 padding, border를 제외한 content영역을 의미, box-sizing : border-box; 를 추가해주면 됨.<br><p>
  <li> CSS 기본파일, nomalize </li>
  <p> body의 margin:0; 이나 div의 box-sizing : border-box; 처럼 기본으로 설정 해두면 좋은 것들을 미리 css상단에 추가해두면 편하다. <br>
  또 브라우저마다 다르게 보이는 문제를 해결하기 위해 CSS normalize라는 문서를 사용할 수 있다. </p>
  <li> form, input </li>
  <p> form에 action과 method로 어떤 경로로 어떤 요청(get, post)을 보낼지 정할 수 있다.<br>
   input type도 정말 다양하게 있고, name으로 서버에 전달. select, option태그로 선택박스 생성가능. 등등... 많으니 필요할 때 검색! </p>
   <li> float </li>
   <p> float 해제시, 부모태그에서 가상요소(::after)를 생성하고<br>
   content:'';<br>
   display:block;<br>
   clear:both;<br>
   을 사용해주면 깔끔하게 가능. </p>

  </ul>
</div>
