# Node.js KEYWORD
<br>

### 🗝 **[1/4일 STUDY KEYWORD](Node.js/keyword01.md)**
```
npm ,webpack ,Node.js ,스레드, noSQL
```
<br>


### * Node.js란?

> #### Node.js는 Chrome V8 JavaScript 엔진으로 빌드 된 JavaScript 런타임입니다.<br>
즉, 노드를 통해 다양한 자바스크립트 애플리케이션을 실행할 수 있으며, 서버를 실행하는 데 제일 많이 사용된다.
- Node.js는 JavaScript를 서버에서도 사용할 수 있도록 만든 프로그램이다.
- Node.js는 V8이라는 JavaScript 엔진 위에서 동작하는 자바스크립트 런타임(환경)이다.
- Node.js는 서버사이트 스크립트 언어가 아니다. 프로그램(환경)이다.
- Node.js는 웹서버와 같이 확장성 있는 네트워크 프로그램을 제작하기 위해 만들어졌다.
- Node.js는 확장성이 있는 네트워크 어플리케이션 개발에 사용되는 소프트웨어 플랫폼이다. 특히 서버사이트에서 많이 사용되고 있다.
- 사용되는 언어로는 자바스크립트(Javascript)를 활용하며, Non-blocking I/O와 단일 스레드 이벤트 루프를 통한 높은 처리 성능을 가지고 있는 것이 특징이다.
<br>

### * Node.js 사용이유?
- #### 한 가지 언어로 전체 웹페이지 구현이 가능함.
- 스크립트 언어는 특정한 프로그램 안에서 동작하는 프로그램이기 때문에 웹 브라우저 프로그램 안에서만 동작을 한다.
- 즉, 웹 브라우저(크롬, 사파리, 익스플로러, 파이어폭스 등)가 없으면 사용할 수 없는 프로그램이다.
- Node.js는 JavaScript 를 웹 브라우저에서 독립시킨 것으로 Node.js를 설치하게 되면 터미널프로그램(윈도우의 cmd, 맥의 terminal 등)에서 Node.js를 입력하여 브라우저 없이 바로 실행할 수 있다.이렇게 Node.js를 이용하여 웹 브라우저와 무관한 프로그램을 만들 수 있게 되었다.
중요한 것은 Node.js를 이용하여 서버를 만들 수 있다는 것이다.
- 중요한 이유는 이전까지 Server-Client 웹사이트를 만들 때 웹에서 표시되는 부분은 JavaScript 를 사용하여 만들어야만 했으며, 서버는 Reby, Java 등 다른 언어를 써서 만들었어야 했는데 마침내 한 가지 언어로 전체 웹 페이지를 만들 수 있게 된 것이다.
<br>

### * 자바스크립트 런타임
- 런타임이란 특정 언어로 만든 프로그램을 실행할 수 있는 환경을 뜻한다.
- 따라서 노드는 자바스크립트 프로그램을 컴퓨터에서 실행할 수 있게 하는 자바스크립트 실행기이다.
<br>

### ❗ Node.js는 이벤트 기반 ( Event-Driven ), 논블로킹 I/O( Non - Blocking I/O), 싱글 스레드 라는 특성❗
<br>

### * 이벤트 기반
- 노드는 V8과 더불어 libuv라는 라이브러리를 사용한다.
- libuv 라이브러리는 노드의 특성인 이벤트 기반, 논 블로킹 I/O 모델을 구현하고 있다.
- 이벤트 기반(Event-driven)이란 이벤트가 발생할 때 미리 지정해둔 작업을 수행하는 방식을 의미한다.
- 즉, 이벤트 기반 시스템에서는 특정 이벤트가 발생할 때 무엇을 할지 미리 등록해두고, 이를 이벤트 리스너에 콜백함수를 등록한다.
- 이후 이벤트가 발생하면 리스너에 등록해둔 콜백함수를 호출하며, 이벤트가 끝난 후 노드는 다음 이벤트가 발생할 때까지 대기한다.
<br>

### * 이벤트 루프
![노드-이벤트루프](https://user-images.githubusercontent.com/76805997/148148312-dd99bb8d-ee81-4cd1-afa2-79c263701857.png)
- 이벤트 루프(event loop)는 여러 이벤트가 동시에 발생했을 때 어떤 순서로 콜백함수를 호출 할지를 이벤트 루프가 판단한다.
- 노드는 이벤트가 종료될 때까지 이벤트 처리를 위한 작업을 반복하므로 루프(loog)라고 부른다.
<br>

### * Non-Blocking I/O
1. Blokcing
- 블로킹(Blocking) I/O는 동작하고 있는 동안에는 다른 일을 처리하지 못하는 상태가 된다.
-  프로그램의 제어권이 호출된 함수가 일을 모두 마무리 될 때까지 넘어가지 않는 것을 이야기한다. 

2. Non-Blocking
- 논 블로킹(Non - Blocking) I/O의 경우, 동작을 한 뒤에 바로 다음 제어가 돌아옴으로써 다음 처리로 넘어갈 수 있게 해준다. 
- (앞서 호출된 함수가 일을 마무리 짓지 않아도 다른 함수가 다른 일을 진행할 수 있도록 해주는 것이다.)
<br>

### * 동기- 비동기
1.동기(Synchronous)
- 호출하는 함수가 호출된 함수의 작업 완료 후 리턴을 기다거나, 호출된 함수로부터 리턴을 받더라도 작업 완료 여부를 호출하는 함수 자체가 계속 체크하는 경우이다.
2. 비동기(Asynchronous) 
- 호출되는 함수에게 CallBack을 전달해서, 호출되는 함수가 작업이 완료되면 호출되는 함수가 이전에 전달받은 CallBack을 실행한다. 호출하는 함수는 작업 완료 여부를 체크하지 않는다.
* 동기와 비동기의 차이점은 호출되는 함수의 완료 여부를 누가 체크하냐에 따라 다르다. 작업 완료를 호출하는 함수 스스로가 계속 체크하면 동기(Synchronous)이며, 작업 완료 여부를 체크하지 않는다면 비동기(Asynchronous) 방식이다.
<br>

cf. 동기/비동기, 블럭/논블럭의 차이점은 동기/비동기의 경우 작업의 결과물을 CallBack인 메시지를 통해 주고 받는데,<br>
작업 완료 여부를 신경쓰는지 안 쓰는지에 따라 차이점이 있으며, 블럭/논블럭의 경우 함수 호출이후에 넘어오는 제어권에 따라 블럭이냐 논블럭이냐를 나누는 것
<br>
<br>

### * 싱글 스레드
- 프로세스 : 운영체제에서 할당하는 작업의 단위이다. 노드나 웹 브라우저 같은 프로그램은 개별적인 프로세스이다. 프로세스 간에는 메모리 등의 자원을 공유하지 않는다.
- 스레드 : 스레드는 프로세스 내에서 실행되는 흐름의 단위이다. 프로세스는 스레드를 여러 개 생성해 여러 작업을 동시에 처리할 수 있다. 스레드들은 부모 프로세스의 자원을 공유한다. 같은 주소의 메모리에 접근 가능하므로 데이터를 공유할 수 있다.

Node.js는 싱글스레드, 논 블로킹 모델로 싱글 스레드가 혼자서 일을 처리하지만 논 블로킹 방식으로 이전 작업이 완료될 때까지 대기하지 않고 다음 작업을 수행한다.

<br>
<br>

### 참고
- [Node.js 이해하기- 싱글스레드](https://dip0cean.tistory.com/7?category=915622)
- [Node.js 이해하기](https://dip0cean.tistory.com/6?category=915622)

<br>
<br>

# node

## node.js 란

- 크롬 V8 자바스크립트 엔진으로 빌드된 자바스크립트 런타임(프로그램을 실행할 수 있는 환경)
- 서버사이트 스크립트 언어 X 프로그램(환경)!!
- 웹서버와 같이 확장성 있는 네트워크 프로그램을 제작하기 위해 만들어짐
- 이벤트기반, 논블로킹 I/O모델을 사용해 가볍고 효율적
- 입문자들은 Node.js가 서버프레임워크 혹은 자바스크립트로 서버를 짜기위해 공부해야하는 무언가로 생각할 수 O → But, **자바스크립트라는 컴퓨터 언어로 만든 프로그램을 실행할 수 있게 만들어주는 환경일뿐 (= 자바스크립트 런타임)**

## node.js 특징

### 부제 - node.js 를 서버로 활용하는 이유

1. 이벤트루프를 활용한 논블로킹 I/O
    
    **이벤트루프**
    
    - **Call Stack이 비어있으면 Callback Queue (Task Queue)에서 함수를 하나씩 가져와 Call Stack에 넣고 실행하는 것**
    - 루프이기때문에 Task Queue에 함수가 대기를 하던 안하던 확인 후 있다면 Call Stack에 넣고 실행을 반복
    - 이벤트기반 - 이벤트가 발생할 때 어떤 순서로 작업을 수행할지 이벤트 루프가 판단
    - 예제 - [http://latentflip.com/loupe](http://latentflip.com/loupe)
    - Call Stack → 코드가 순차적으로 읽히면서 쌓이게되는 영역
    - Web Apis(Background) → 콜백 또는 이벤트 리스너들이 Call Stack에서 읽힌 후 대기하는 영역
    - Callback Queue (Task Queue) → Web Apis(Background)에서 작업이 완료되면 호출되어야할 함수들이 대기하는 영역
    
    **논블로킹**
    
    - **이전 작업이 완료될때까지 멈춰져있지 않고 다음작업을 실행하는 것**
    - 비동기?
2. 싱글스레드
    - 스레드 → 프로세스 내에서 실행되는 흐름의 단위이며 부모프로세스의 자원을 공유
    - 프로세스 → 운영체제에서 할당하는 작업의 단위이며 쉽게말해 실행중인 프로그램
    - 자바스크립트와 Node.js는 싱글스레드
    - 하나의 작업만 처리할 수 있지만, **이벤트루프를 활용한 논블로킹I/O를 통해 고성능 병렬처리가 가능**
    - 싱글스레드이므로 시간(연산)이 오래걸리는 작업을 한다면 서버전체의 성능이 저하 (cluster, pm2를 사용하여 멀티프로세싱 혹은 AWS Lambda, Google Cloud Function으로 해소 가능)
    
    멀티스레드 단점
    
    - 스레드가 증가할수록 비용 증가
    - 서버자원은 한정적이기 때문에 동시접속자만큼 스레드를 증가시킬 수 없음 (서버를 업그레이드하거나 Load-Balancing으로 해소 가능)
    - 자원을 공유하기때문에 공유자원 접근 문제가 발생 / thread-unsafe라고 표현하기도 함
3. 자바스크립트이기 때문에 프론트와 백을 하나의 언어로 개발할 수 O

 

# 참고자료
    
- node.js
    
    [https://medium.com/@seungh93/node-js-이해하기-기초-입문-b5af7aed374c](https://medium.com/@seungh93/node-js-%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0-%EA%B8%B0%EC%B4%88-%EC%9E%85%EB%AC%B8-b5af7aed374c)
    
    [https://hanamon.kr/nodejs-개념-이해하기/](https://hanamon.kr/nodejs-%EA%B0%9C%EB%85%90-%EC%9D%B4%ED%95%B4%ED%95%98%EA%B8%B0/)