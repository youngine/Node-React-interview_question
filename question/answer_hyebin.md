## 📃 기술 외 공통 면접 질문

### [ 자기소개 및 지원동기 ]

### [ 주요 기술스택 및 역할 ] ✅

FE

- React
- 사용한 React library
    - react-chartjs-2
    - react-redux
    - redux-thunk
    - reactstrap
    - react-leaflet

BE

- node.js(Express)
- mongoDB

버전관리

- Git / Github

역할

- redux를 이용한 회원관리(로그인, 로그아웃, 회원가입)구현
- cors 미들웨어를 이용해서 공공데이터 API 요청
- 공공데이터 요청 및 응답 데이터 전처리
- 국가 여행 정보 검색페이지 구현
    - OpenWheatrherMap API를 이용해서 해당 국가 날씨 정보 제공
    - 공공데이터 API를 이용해서 해당국가 코로나 관련 정보 제공
    - 그래프를 활용해서 데이터 시각화(react-chartjs-2 사용)

### [ 자기소개서 기반의 프로젝트 질문 ] ✅

- 어떤 역할을 담당하였는가? ✅
    - 위에 작성
- 서버는 어떻게 구성하였는가? ✅
    - Node.js 웹 애플리케이션 프레임워크인 Express를 활용해서 RESTful API 서버를 구축
    - express 기반 웹 서버 구동
- 어떤 언어와 프레임워크, 라이브러리? ✅
    - react,node.js
- 몇명의 사용자, 어느 정도의 트래픽 ✅
    - 공공데이터 포털 API가 하루 1000건으로 제한되어 있었고 운영 신청을 하면 제한이 없어지지만, 여러 사용자가 함께 사용해보는 테스트를 하지 못했습니다.

    **사용자가 많다면 어떻게 서버를 구성해서 트래픽을 관리해야할까?**

    - node.js를 통해 구현한 server 환경에서 분산처리가 중요한 이유 중 하나는 node.js가 싱글스레드 구조이기 때문이다.
    
    ![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/73d23412-fef6-4e6e-9445-a6f462e736c5/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220126%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220126T050052Z&X-Amz-Expires=86400&X-Amz-Signature=7776e58527f97fa72115b4598671b17dcd47cb5f6163422b08a7712c856d8ae6&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)
    
    **참고**
    
    - [https://velog.io/@gyrbs22/node.js-node.js를-활용하는-서버환경의-이해](https://velog.io/@gyrbs22/node.js-node.js%EB%A5%BC-%ED%99%9C%EC%9A%A9%ED%95%98%EB%8A%94-%EC%84%9C%EB%B2%84%ED%99%98%EA%B2%BD%EC%9D%98-%EC%9D%B4%ED%95%B4)
    - [https://velog.io/@therichu/Nodejs-에서-고비용대용량-연산하기-성능편](https://velog.io/@therichu/Nodejs-%EC%97%90%EC%84%9C-%EA%B3%A0%EB%B9%84%EC%9A%A9%EB%8C%80%EC%9A%A9%EB%9F%89-%EC%97%B0%EC%82%B0%ED%95%98%EA%B8%B0-%EC%84%B1%EB%8A%A5%ED%8E%B8)
    - [https://www.nextree.co.kr/p7292/](https://www.nextree.co.kr/p7292/)
- 해당 기술 스택을 사용한 이유 ✅
    - 자바스크립트 언어 하나로 프론트 엔드, 벡앤드 모두 구현할 수 있기 때문에 단시간에 완성해야하는 프로젝트에 적합하다고 생각했습니다.
- 구조에 대한 설명 및 설계 관련 내용 ✅
    - 어떤 내용을 작성해야하는거지.....?
    - 여행 종합 도표 페이지
    - 국가 여행 정보 페이지
    - 여행 경보 페이지
    - 찜한 국가 페이지
- 어떠한 알고리즘, 자료구조 혹은 디자인패턴을 사용하였는가?
- 개선점은 무엇이였나? ✅
    - **개선할 점**
    - 코드 리팩토링(클린코드)
    - 코드 컴포넌트화(데이터 처리하는 부분과 UI부분 소스 분리)
    - 디비에 데이터를 요청하고 받아오는 부분이 비동기 처리 되지만, 동기처리 되도록하여 데이터 불러오는게 오래걸려서 화면 로딩이? 오래 걸리는 부분을 수정해야합니다.
- 어떻게 프로젝트를 관리했고(스케줄, 소통 등) 어떻게 기여했는가?(문서화, 구조 설계, 개발 등) ✅
    - notion으로 to do list를 만들어서 스케줄 관리를 하였습니다.
    - github를 이용해서 코드를 지속적으로 통합하고 관리했습니다.
- 자신의 프로젝트에서 다양한 상황을 가정해보자. (이런 경우 혹은 저런 경우엔 어떻게 하실 건가요? 같은 질문을 자주 함)
