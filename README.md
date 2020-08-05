# Mask-project
마스크 알리미 프로젝트

**웹을 공부하면서 흔하게 접하는 용어 정리**
---------------------------------------------------
## ❤️API
서비스를 개발할 때, 서비스를 사용하기 위한 규칙 또는 규약
ex) 하우징 맵 
- 지도를 설정하는 것이 너무 번거로워 구글지도 위에 부동산 정보를 띄우는 것

만약 기업이 API를 제공하지 않으면?
파싱 등을 이용하여 직접 코딩해야 한다.

* SOAP API vs REST API
1. SOAP API
유형 : 프로토콜
데이터 포멧 : XML만 사용
SOAP는 그 자체로 프로토콜 이며, 보안이나 메시지 전송 등에 있어서 REST보다 더 많은 표준들이 정해져있기 때문에 조금 더 복잡하다.

2. REST API
유형 : 아키텍처 스타일
데이터 포멧 : 일반 텍스트, HTML, XML, JSON등 다양한 포맷을 허용
REST는 네트워크를 통해서 컴퓨터들끼리 통신할 수 있게 해주는 아키텍처 스타일이다.
REST API는 URL과 HTTP프로토콜을 기반으로 한다. 데이터 포맷으로는 브라우저 간 호환성이 좋은 JSON을 사용한다.
REST API는 구축과 확장이 간단하지만, 크고 복잡하게 만들 수도 있다.

* URL의 구성
1. 프로토콜  http, https, file 등
2. 호스트 주소 www.naver.com, www.google.com
3. 파일 경로 /home, /index.html
4. Query parameter ?id = 1&postld =1 (검색, 필터링, 데이터 교환 시 사용)

## 🧡HTTP
HTML문서를 교환하기 위해 만들어진 통신규약
프론트엔드 서버와 클라이어느간의 통신, 백엔드와 프론트엔드 서버간의 통신에 사용되며, TCP/IP 기반으로 되어있다.

* HTTP 통신 방식
요청(request) / 응답(response) 구조로 되어있다.
- 클라이언트가 HTTP request를 서버에 보내면 서버는 HTTP response를 보내는 구조이다.
- 클라이언트와 서버의 모든 통신은 요청과 응답으로 이루어진다.

* HTTP의 요청 메소드
1. GET - UTL에 표시된 리소스를 가져오기
2. POST - body에 정보를 담아 서버에 입력
3. PUT - URL에 표시된 리소스와 바꿔치기
4. PATCH - PUT과 다르게 일부만 수정
5. DELETE - URL에 표시된 특정 리소스를 삭제

## 💛JSON
- JSON은 경량의 DATA-교환 형식
---------------------------------------------------------------------------------
**💚Javascript 기초 문법**
* 자습할때 참고하기 좋은 페이지
1. W3C School : https://www.w3schools.com/
2. MDN Document : https://developer.mozilla.org/ko/docs/Web/JavaScript
3. 생활코딩 WEB2 - Javascript : https://opentutorials.org/course/3085
4. ofcourse : https://ofcourse.kr/

* 변수
> 사용가능한 데이터 타입 : Boolean, Null, Undefined, Number, String, Symbol, Object
> var : 변수
> let : block scope 변수
> const : 변하지 않는 데이터를 저장


* Javascript 사용법  
1. HTML 내부에서 <script> 태그내에서 사용
2. js. 파일로 만들고, <script src = "파일경로">를 사용해서 불러옴
  
* 비동기 처리
> promise 객체를 사용한다.
1. 대기
2. 이행
3. 거부

* Fetch API
1. Fetch API는 네트워크 통신을 위해서 제공되는 API이다.
2. promise객체를 반환한다.
3. request, response 라는 두 개의 객체를 사용한다.

## UI작업, Kakao Map 삽입
1. HTML 구조 만들기
>Navbar 
>Main

2. 기본으로 들어있는 스타일 제거
> 기본적으로 html, body에 margin이 들어있다.
> 그대로 나두게 되면 꽉찬 화면을 만들 수 없다.
> body, html이 전체화면을 채우도록 크기를 지정해준다.

3. Navbar 만들기
> 적당한 색깔로 만들어 준다.
> 투명도를 주어 뒤에 Map도 보일 수 있도록 해준다.

* opacity - 투명도 설정
* ctrl + shift - 주석처리 가능
* width, height - 사이즈 설정
* ex) position : absolute - 위치 설정(고정설정)
*<script></script> - 태그를 만들어서 Java script를  삽입


4. Fontawesome CDN 추가
>Fontawesome은 아이콘 폰트를 제공해주는 사이트이다.
> 여기서 Back button과 유사한 것을 찾아서 넣어줄 것이다.

5. Navbar에 Back button 추가하기
> 위치는 왼쪽에 고정
> 색은 흰색
> 사이즈 조절해서 적당한 크기로 만들어준다.

6. Kakao 지도 추가하기
> API키를 발급하기
> kakao developers 이용
> 지도를 추가한 후, 지도 크기/ 위치 조정

7. 검색 창 만들기
> 검색창 구조
* 검색창 전체 위치를 조정해줄 컨테이너
* 검색창을 감싸고 있는 배경
* 검색창의 input
* 검색버튼
> 검색창 폰트를 나눔고딕으로 바꾸기 위해 웹폰트 가져오기
> 웹폰트 적용하기

* . vs #의 차이점
> # 기호는 HTML id 속성을 CSS 선택자로 지정할 때 id명 앞에 붙이는 기호
> . 기호는 HTML class 속성을 CSS 선택자로 지정할 때 class명 앞에 붙이는 기호입니다.

# 메인 화면 기능 구현
* 검색 기능
* 마스크 데이터를 불러와서 Marker그리기
* Mask 수량에 따라 다른 Marker 띄우기
* Marker 클릭 시 정보 띄우기

# 시작화면 UI 및 기능 구현
* 화면 UI만들기
* 메인 화면의 기능과 연결하기
*추가기능 - 목록보기 만들어 보기
