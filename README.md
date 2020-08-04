# Mask-project
마스크 알리미 프로젝트

**웹을 공부하면서 흔하게 접하는 용어 정리**
## API
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

## HTTP
HTML문서를 교환하기 위해 만들어진 통신규약
프론트엔드 서버와 클라이어느간의 통신, 백엔드와 프론트엔드 서버간의 통신에 사용되며, TCP/IP 기반으로 되어있다.

* HTTP 통신 방식
요청(request) / 응답(response) 구조로 되어있다.
- 클라이언트가 HTTP request를 서버에 보내면 서버는 HTTP response를 보내는 구조이다.
- 클라이언트와 서버의 모든 통신은 요청과 응답으로 이루어진다.

* HTTP의 요청 메소드
GET - UTL에 표시된 리소스를 가져오기
POST - body에 정보를 담아 서버에 입력
PUT - URL에 표시된 리소스와 바꿔치기
PATCH - PUT과 다르게 일부만 수정
DELETE - URL에 표시된 특정 리소스를 삭제

* JSON
- JSON은 경량의 DATA-교환 형식
