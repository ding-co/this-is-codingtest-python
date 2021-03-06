# 개발형 코딩 테스트

## 개발형 코딩 테스트에 필요한 지식

### 알고리즘 코딩 테스트 vs. 개발형 코딩 테스트

- 알고리즘 코딩 테스트
  - 한정된 컴퓨터 자원 활용, 정해진 시간 안에 정확하게 동작하는 효율적인 프로그램 작성
  - 요구사항에 맞게 효율적으로 동작하는 모듈 개발
- 개발형 코딩 테스트
  - 정해진 목적에 따라서 동작하는 완성된 프로그램 개발
  - 모듈을 적절히 조합하여 완성도 높은 프로그램 개발
  - 분야에 따라 구체적인 요구사항이 다름
  - 대부분 서버와 클라이언트로 기능 나눠 개발

### 서버와 클라이언트

- 서버
  - 서버는 클라이언트에게 정보 응답
  - ex) 음식점 - 음식 접대하는 사람
  - 정보 생성 및 보내주는 역할은 서버가 함
  - 클라이언트에게 서비스 제공해주는 컴퓨터
  - 서버 프로그램은 사용자의 요청에 대한 특정한 작업 수행 목적
  - 서버는 요청 받은 작업을 서버 프로그램으로 실행한 다음 <br/>
    결과를 클라이언트 프로그램에 응답으로 보내줌
- 클라이언트
  - 클라이언트가 서버에게 정보 요청
  - ex) 음식점 - 손님
  - 출력만 담당
- HTTP
  - 웹 상에서 데이터를 주고 받기 위한 프로토콜
  - 대표 4가지 HTTP 메서드 (REST 아키텍쳐에 맞는 각 메서드별 기능)
    - GET; 특정 데이터 조회 요청
      - ex) 특정 페이지 접속, 정보 검색
    - POST; 특정 데이터 생성 요청
      - ex) 회원가입, 글쓰기
    - PUT; 특정 데이터 수정 요청
      - ex) 회원 정보 수정
    - DELETE; 특정 데이터 삭제 요청
      - ex) 회원 정보 삭제

### REST API란?

- REpresentational State Transfer
  - 각 자원에 대하여 자원의 상태에 대한 정보 주고받는 개발 방식
  - 서버의 자원을 어떠한 방식으로 접근하도록 해야 하는지 구체적으로 명시
  - HTTP 프로토콜 그대로 사용
- API
  - 프로그램이 상호작용하기 위한 인터페이스
- REST API
  - REST 아키텍쳐를 따르는 API
- REST API 호출 (클라이언트 입장)
  - REST 방식을 따르고 있는 서버에 특정한 요청 보내서 데이터 가져오기
- REST 이용 방법
  - HTTP URI로 자원 명시
  - HTTP 메서드로 해당 자원 어떻게 처리할 것인지 명시
- REST 구성 요소
  - 자원(Resource); URI 이용하여 표현, 명사 형태 이용
  - 행위(Verb); HTTP 메서드 이용하여 표현
  - 표현(Representations)
- JSON
  - JavaScript Object Notation
  - 데이터의 형식에 대한 표준
  - 데이터를 주고받는데 사용하는 경량의 데이터 형식 (데이터 주고받는 형식일 뿐)
  - JSON 데이터는 키-값 쌍으로 이루어진 데이터 객체 저장
  - JSON 인코딩; 파이썬의 기본 자료형을 JSON 객체로 변환
    - json.dumps() 메서드 이용하여 JSON 객체 생성
  - JSON 디코딩; JSON 객체를 파이썬의 기본 자료형으로 변환
    - json.loads() 메서드 이용
- 파이썬으로 REST API 호출 실습
  - JSON 목킹 사이트 이용

### 개발형 코딩 테스트 준비 방법

- 자신이 실제로 맡고 싶은 직무와 관련된 애플리케이션 개발해보기
  - ex) 회원 관리 애플리케이션 개발
  - 서버 쪽에서 REST API 개발
  - 클라이언트쪽에서 REST API 호출

#

### [Note]

- 프레임워크; 어떠한 프로그램을 개발하기 위한 바탕이 되는 템플릿과 같은 역할을 하는 소스코드 집합
- CRUD; Create, Read, Update, Delete
- Payload; 실제 데이터
  - 인터넷에서 데이터 보낼 때, 속성 표현하는 헤더와 전달해야 하는 실제 데이터인 페이로드
- 목킹; 어떠한 기능이 있는 것처럼 흉내내어 구현한 것
- 파싱; 특정한 형식으로 저장된 데이터에 접근하여 원하는 정보만 찾아서 가공하는 작업
