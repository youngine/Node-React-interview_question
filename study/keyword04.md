# KEYWORD 04
<br>


### 🗝 **[1/6일 STUDY KEYWORD](study/keyword04.md)**
```
block/nonblock, 동기/비동기, 프로세스/스레드, 총 복습, noSQL
```

<br>

### * 데이터베이스란?
- 데이터베이스란 데이터의 모음을 말한다.
- 일반적으로 컴퓨터 시스템에 전자적으로 저장되는 조직화된 데이터 모음을 말한다.
- 이렇게 데이터를 조직화하면 데이터에 의미가 생긴다. 또한 대량의 데이터를 효율적으로 관리할 수 있다.
<br>

### *데이터베이스 관리 시스템 (DBMS)?
- 이러한 개념적인 데이터베이스를 실질적으로 구현하기 위해서 일반적으로 데이터베이스 관리 시스템 (DBMS) 이라는 것을 사용한다.
- 연결할 애플리케이션, 데이터, DBMS 솔루션을 하나로 묶어 데이터베이스 시스템이라고 하고 단축해서 데이터베이스라고도 한다.
<br>

### *관계형 데이터베이스?
- 데이터베이스 유형 중에 관계형 데이터베이스가 있다.
- 관계형 데이터베이스는 고정된 행(row)과 열(column)로 구성된 테이블에 데이터를 저장한다.
- 각 열은 하나의 속성에 대한 정보를 저장하고, 행에는 각 열의 데이터 형식에 맞는 데이터가 저장된다.
- 관계형 데이터베이스에서는 테이블의 구조와 데이터 타입 등을 사전에 정의한다. 그리고 테이블에 정의된 내용에 알맞은 형태의 데이터만 삽입할 수 있다.
- 특정한 형식을 지키기 때문에, 데이터를 정확히 입력했다면 데이터를 사용할 때에는 매우 수월하다.
<br>

### *관계형 데이터베이스 관리 시스템?
- 관계형 데이터베이스의 대표적인 DBMS는 아래와 같다.
- 관계형 데이터베이스 관리 시스템을 따로 RDBMS라고 부른다.
- MySQL
- Oracle
- SQLite
- MariaDB
- PostgresSQL
<br>

### *관계형 데이터베이스는 SQL 사용
- 관계형 데이터베이스와 상호작용할 때 SQL 사용할 수 있다.
- 이 말은 관계형 데이터베이스에서는 스키마가 뚜렷하게 보인다는 말과 같다.
- 다시 말해, 관계형 데이터베이스에서는 테이블 간의 관계를 직관적으로 파악할 수 있다.

<br>

>### 👉 즉, SQL 관계형 DB 는
- 데이터베이스 유형 중 관계형 데이터베이스는 테이블 기반으로 데이터를 저장한다. 그리고 SQL을 사용해서 데이터를 다룰 수 있다.
- 테이블의 관계가 구조화된 데이터의 모음이기 때문에 구조화된 쿼리 언어를 사용할 수 있는 것이다.
<br>

### * 비관계형 데이터베이스?
- 비관계형 데이터베이스란 관계형 데이터베이스를 뺀 나머지 유형을 총칭하는 뜻이다.
- 관계형 데이터베이스를 SQL이라고 칭하는 것과 마찬가지로 비관계형 데이터베이스를 칭할 때 NoSQL(또는 NoSQL 데이터베이스)라고 한다.
- 그런데 주의할 점은 NoSQL 데이터베이스 또는 비관계형 데이터베이스로도 관계 데이터를 저장할 수 있다. (관계형 데이터베이스와 방식은 다르지만)
<br>

### * NoSQL 데이터베이스는 ?
- NoSQL 데이터베이스(일명 “SQL만을 사용하지 않는 데이터베이스”)는 표 형식이 아니며, 관계형 테이블과는 다른 방식으로 데이터를 저장한다.
- NoSQL 데이터베이스는 SQL 앞에 붙은 ‘No’에서 알 수 있듯이, 주로 데이터가 고정되어 있지 않은 데이터베이스를 가리킨다.
- NoSQL 데이터베이스는 데이터 모델에 따라 유형이 다양하다.
- 주요 유형으로는 문서, 키 값, 와이드 컬럼, 그래프가 있다.
- NoSQL이 SQL과 반대되는 개념처럼 사용된다고 해서, NoSQL에 스키마가 반드시 없는 것은 아니다.
- 이들은 유연한 스키마를 제공하며, 대량의 데이터와 높은 사용자 부하에서도 손쉽게 확장이 가능하다.
- 관계형 데이터베이스에서는 데이터를 입력할 때 스키마에 맞게 입력해야 하는 반면, NoSQL에서는 데이터를 읽어올 때 스키마에 따라 데이터를 읽어 온다.
- 이런 방식을 ‘schema on read’라고도 한다.
- 읽어올 때에만 데이터 스키마가 사용된다고 하여, 데이터를 쓸 때 정해진 방식이 없다는 의미는 아니다.
- 데이터를 입력하는 방식에 따라, 데이터를 읽어올 때 영향을 미친다.
<br>

### * ❗️SQL 데이터베이스와 NoSQL 데이터베이스 차이점

#### 1. 데이터 저장(Storage)
- NoSQL은 key-value, document, wide-column, graph 등의 방식으로 데이터를 저장한다.
- 관계형 데이터베이스는 SQL을 이용해서 데이터를 테이블에 저장한다.
- 미리 작성된 스키마를 기반으로 정해진 형식에 맞게 데이터를 저장해야 한다.

#### 2. 스키마(Schema)
- SQL을 사용하려면, 고정된 형식의 스키마가 필요하다.
- 다시 말해, 처리하려는 데이터 속성별로 열(column)에 대한 정보를 미리 정해두어야 한다.
- 스키마는 나중에 변경할 수 있지만, 이 경우 데이터베이스 전체를 수정하거나 오프라인(down-time)으로 전환할 필요가 있다.
- NoSQL은 관계형 데이터베이스보다 동적으로 스키마의 형태를 관리할 수 있다.
- 행을 추가할 때 즉시 새로운 열을 추가할 수 있고, 개별 속성에 대해서 모든 열에 대한 데이터를 반드시 입력하지 않아도 된다.

#### 3. 쿼리(Querying)
- 쿼리는 데이터베이스에 대해서 정보를 요청하는 질의문이다.
- 관계형 데이터베이스는 테이블의 형식과 테이블간의 관계에 맞춰 데이터를 요청해야 한다.
- 그래서 정보를 요청할 때, SQL과 같이 구조화된 쿼리 언어를 사용한다.
- 비관계형 데이터베이스의 쿼리는 데이터 그룹 자체를 조회하는 것에 초점을 두고 있다.
- 그래서 구조화 되지 않은 쿼리 언어로도 데이터 요청이 가능하다.
- UnQL(UnStructured Query Language)이라고 말하기도 한다.

#### 4. 확장성(Scalability)
- 일반적으로 SQL 기반의 관계형 데이터베이스는 수직적으로 확장하다.
- 높은 메모리, CPU를 사용하는 확장이라고도 한다.
- 데이터베이스가 구축된 하드웨어의 성능을 많이 이용하기 때문에 비용이 많이 든다.
- 여러 서버에 걸쳐서 데이터베이스의 관계를 정의할 수 있지만, 매우 복잡하고 시간이 많이 소모된다.
- NoSQL로 구성된 데이터베이스는 수평적으로 확장한다.
- 보다 값싼 서버 증설, 또는 클라우드 서비스 이용하는 확장이라고도 한다.
- NoSQL 데이터베이스를 위한 서버를 추가적으로 구축하면, 많은 트래픽을 보다 편리하게 처리할 수 있다.
- 그리고 저렴한 범용 하드웨어나 클라우드 기반의 인스턴스에 NoSQL 데이터베이스를 호스팅할 수 있어서, 수직적 확장보다 상대적으로 비용이 저렴하다
<br>

### * ❗️SQL 기반의 관계형 데이터베이스를 사용하는 케이스
#### 1. 데이터베이스의 ACID 성질을 준수해야 하는 경우
- ACID는 Atomicity(원자성), Consistency(일관성), Isolation(격리성), Durability(지속성) 를 의미한다.
- 각 단어는 데이터베이스에서 실행되는 하나의 트랜잭션(Transaction)에 의한 상태의 변화를 수행하는 과정에서, 안전성을 보장하기 위해 필요한 성질이다.
- SQL을 사용하면 데이터베이스와 상호 작용하는 방식을 정확하게 규정할 수 있기 때문에, 데이터베이스에서 데이터를 처리할 때 발생할 수 있는 예외적인 상황을 줄이고, 데이터베이스의 무결성을 보호할 수 있다.
- 전자 상거래를 비롯한 모든 금융 서비스를 위한 소프트웨어 개발 에서는 반드시 데이터베이스의 ACID 성질을 준수해야 한다.
- 그래서 이런 경우에는 일반적으로 SQL을 이용한 관계형 데이터베이스를 사용한다.
#### 2. 소프트웨어에 사용되는 데이터가 구조적이고 일관적인 경우
- 소프트웨어(프로젝트)의 규모가 많은 서버를 필요로 하지 않고 일관된 데이터를 사용하는 경우, 관계형 데이터베이스를 사용하는 경우가 많다.
- 다양한 데이터 유형과 높은 트래픽을 지원하도록 설계된 NoSQL 데이터베이스를 사용해야만 하는 이유가 없기 때문이다.
 <br>

### * ❗️NoSQL 기반의 비관계형 데이터베이스를 사용하는 케이스
#### 1. 데이터의 구조가 거의 또는 전혀 없는 대용량의 데이터를 저장하는 경우
- 대부분의 NoSQL 데이터베이스는 저장할 수 있는 데이터의 유형에 제한이 없다.
- 필요에 따라, 언제든지 데이터의 새 유형을 추가할 수 있다.
- 소프트웨어 개발에 정형화 되지 않은 많은 양의 데이터가 필요한 경우, NoSQL을 적용하는 것이 더 효율적일 수 있다.
#### 2. 클라우드 컴퓨팅 및 저장공간을 최대한 활용하는 경우
- 클라우드 기반으로 데이터베이스 저장소를 구축하면, 저렴한 비용의 솔루션을 제공받을 수 있다.
- 소프트웨어에 데이터베이스의 확장성이 중요하다면, 별다른 번거로움 없이 확장할 수 있는 NoSQL 데이터베이스를 사용하는 것이 좋다.
3. 빠르게 서비스를 구축하는 과정에서 데이터 구조를 자주 업데이트 하는 경우
- NoSQL 데이터베이스의 경우 스키마를 미리 준비할 필요가 없기 때문에 빠르게 개발하는 과정에 매우 유리하다.
- 시장에 빠르게 프로토타입을 출시해야 하는 경우가 이에 해당한다.
- 또한 소프트웨어 버전별로 많은 다운타임(데이터베이스 서버를 오프라인으로 전환하여 데이터 처리를 진행하는 작업 시간) 없이 데이터 구조를 자주 업데이트 해야하는 경우, 스키마를 매번 수정해야 하는 관계형 데이터베이스 보다 NoSQL 기반의 비관계형 데이터베이스를 사용하는 게 더 적합하다.
<br>

### * sql vs nosql?
![1](https://user-images.githubusercontent.com/76805997/148506252-ab414ae3-2ad2-4a15-8fe9-c63c584c77d3.PNG)
![2](https://user-images.githubusercontent.com/76805997/148506257-098194fb-0ec1-4889-833f-548bc152d9a2.PNG)
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
- [SQL(구조화 쿼리 언어) vs NoSQL(비구조화 쿼리 언어)](https://hanamon.kr/%EB%8D%B0%EC%9D%B4%ED%84%B0%EB%B2%A0%EC%9D%B4%EC%8A%A4-sql-vs-nosql/)
- [멀티프로세스 & 멀티스레드 이해하기](https://wooody92.github.io/os/%EB%A9%80%ED%8B%B0-%ED%94%84%EB%A1%9C%EC%84%B8%EC%8A%A4%EC%99%80-%EB%A9%80%ED%8B%B0-%EC%8A%A4%EB%A0%88%EB%93%9C/)

<br>
<br>

## blocking, non blocking, sync, async

호출한 함수가 호출된 함수의 작업이 끝나서 **결과값을 반화하기를 기다리거나**, **지속적으로 호출된 함수에게 확인 요청을하는 경우**

### Blocking/NonBlocking

- **Blocking/NonBlocking은 호출되는 함수가 바로 리턴하느냐 마느냐**
- 호출되는 대상이 직접 제어할 수 없는 경우 이를 구분할 수 있다
- **Blocking** → 호출된 함수가 자신의 작업을 모두 마칠 때까지 호출한 함수에게 제어권을 넘겨주지 않고 대기하게 만든다면
- **NonBlocking** → 호출된 함수가 바로 리턴해서 호출한 함수에게 제어권을 넘겨주고, 호출한 함수가 다른 일을 할 수 있는 기회를 줌

### Synchronous/Asynchronous

- **Synchronous/Asynchronous는 호출되는 함수의 작업 완료 여부를 누가 신경쓰냐**
- 두 가지 이상의 대상(메서드, 작업, 처리 등)과 이를 처리하는 시간으로 구분한다
- **Synchronous** → 호출하는 함수가 호출되는 함수의 작업 완료 후 리턴을 기다리거나, 또는 호출되는 함수로부터 바로 리턴 받더라도 작업 완료 여부를 호출하는 함수 스스로 계속 확인하며 신경씀
- **Asynchronous** → 호출되는 함수에게 callback을 전달해서, 호출되는 함수의 작업이 완료되면 호출되는 함수가 전달받은 callback을 실행하고, 호출하는 함수는 작업 완료 여부를 신경쓰지 않음

## callback 함수

- **called at the back**

콜백 함수란

1. 다른 함수의 인자로써 이용되는 함수
2. 어떤 이벤트에 의해 호출되어지는 함수

## 프로세스, 스레드

### 프로세스

- 사전적 의미 → 어떤 작업을 위해 실행할 수 있는 파일
- 사전적 의미
    - “컴퓨터에서 연속적으로 실행되고 있는 컴퓨터 프로그램”
    - 메모리에 올라와 실행되고 있는 프로그램의 인스턴스(독립적인 개체)
    - 운영체제로부터 시스템 자원을 할당받는 작업의 단위
    - 즉, 동적인 개념으로는 실행된 프로그램
- 참고 할당받는 시스템 자원의 예
    - CPU 시간
    - 운영되기 위해 필요한 주소 공간
    - Code, Data, Stack, Heap의 구조로 되어 있는 독립된 메모리 영역
- 특징
    
    ![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/0f915355-0064-40d6-a1c9-b17e211bc9d2/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T083122Z&X-Amz-Expires=86400&X-Amz-Signature=6a7fc8e0606935f8ba1a9807b36a27b92a71bff9daca1a8f399d4938428f9042&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)
    
    - 프로세스는 각각 독립된 메모리 영역(Code, Data, Stack, Heap의 구조)을 할당받음
    - **기본적으로 프로세스당 최소 1개의 스레드(메인 스레드)를 가지고 있음**
    - 각 프로세스는 별도의 주소 공간에서 실행되며, 한 프로세스는 다른 프로세스의 변수나 자료구조에 접근할 수 없음
    - 한 프로세스가 다른 프로세스의 자원에 접근하려면 **프로세스 간의 통신**(IPC, inter-process communication)을 사용해야 함
    - Ex. 파이프, 파일, 소켓 등을 이용한 통신 방법 이용

### 스레드

- 사전적 의미
    - “**프로세스 내**에서 실행되는 여러 흐름의 단위”
    - 프로세스의 특정한 수행 경로
    - 프로세스가 할당받은 자원을 이용하는 실행의 단위
- 특징
    
    ![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/cfab3254-ae0b-4ecd-8991-72848f4d67a6/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T083139Z&X-Amz-Expires=86400&X-Amz-Signature=aad366322aaa8e598d22475aaebcb5ec39415d017295cd4fe34e4c39276f2051&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)
    
    - 스레드는 프로세스 내에서 각각 Stack만 따로 할당받고 Code, Data, Heap 영역은 공유
    - 스레드는 **한 프로세스 내에서 동작되는 여러 실행의 흐름**으로, 프로세스 내의 주소 공간이나 자원들(힙 공간 등)을 같은 프로세스 내에 스레드끼리 공유하면서 실행
    - 같은 프로세스 안에 있는 여러 스레드들은 같은 힙 공간을 공유
    - 반면에 프로세스는 다른 프로세스의 메모리에 직접 접근할 수 없음
    - 각각의 스레드는 별도의 레지스터와 스택을 갖고 있지만, 힙 메모리는 서로 읽고 쓸 수 있음
    - **한 스레드가 프로세스 자원을 변경하면, 다른 이웃 스레드(sibling thread)도 그 변경 결과를 즉시 볼 수 있음**

### 멀티프로세스와 멀티 스레드 차이

### 멀티 프로세스

- 멀티 프로세싱이란
    - 하나의 응용프로그램을 여러 개의 프로세스로 구성하여 **각 프로세스가 하나의 작업(태스크)을 처리**하도록 하는 것
- 장점
    - 여러 개의 자식 프로세스 중 하나에 문제가 발생하면 그 자식 프로세스만 죽는 것 이상으로 다른 영향이 확산되지 않음
- 단점
    - Context Switching에서의 오버헤드
        - Context Switching 과정에서 캐쉬 메모리 초기화 등 무거운 작업이 진행되고 많은 시간이 소모되는 등의 오버헤드가 발생
        - 프로세스는 각각의 독립된 메모리 영역을 할당받았기 때문에 프로세스 사이에서 공유하는 메모리가 없어, Context Switching가 발생하면 **캐쉬에 있는 모든 데이터를 모두 리셋하고 다시 캐쉬 정보를 불러와야 함**
    - 프로세스 사이의 어렵고 복잡한 통신 기법(IPC)
        - 프로세스는 각각의 독립된 메모리 영역을 할당받았기 때문에 하나의 프로그램에 속하는 프로세스들 사이의 변수를 공유할 수 없음
- 참고 **Context Switching란?**
    - **CPU에서 여러 프로세스를 돌아가면서 작업을 처리하는 데 이 과정**
    - 구체적으로, 동작 중인 프로세스가 대기를 하면서 해당 프로세스의 상태(Context)를 보관하고, 대기하고 있던 다음 순서의 프로세스가 동작하면서 이전에 보관했던 프로세스의 상태를 복구하는 작업

### 멀티스레드

- 멀티 스레딩이란
    - **하나의 응용프로그램을 여러 개의 스레드로 구성**하고 **각 스레드로 하여금 하나의 작업을 처리**하도록 하는 것
    - 윈도우, 리눅스 등 많은 운영체제들이 멀티 프로세싱을 지원하고 있지만 멀티 스레딩을 기본으로 하고 있음
    - 웹 서버는 대표적인 멀티 스레드 응용 프로그램
- 장점
    - 시스템 자원 소모 감소 (자원의 효율성 증대)
        - 프로세스를 생성하여 자원을 할당하는 시스템 콜이 줄어들어 자원을 효율적으로 관리
    - 시스템 처리량 증가 (처리 비용 감소)
        - 스레드 간 데이터를 주고 받는 것이 간단해지고 시스템 자원 소모가 줄어들게 됨
        - 스레드 사이의 작업량이 작아 Context Switching이 빠름
    - 간단한 통신 방법으로 인한 프로그램 응답 시간 단축
        - 스레드는 프로세스 내의 Stack 영역을 제외한 **모든 메모리를 공유**하기 때문에 통신의 부담이 적음
- 단점
    - 주의 깊은 설계가 필요
    - 디버깅이 까다로움
    - 단일 프로세스 시스템의 경우 효과를 기대하기 어려움
    - 다른 프로세스에서 스레드를 제어할 수 없음(즉, 프로세스 밖에서 스레드 각각을 제어할 수 없음)
    - 멀티 스레드의 경우 자원 공유의 문제가 발생 (동기화 문제)
    - 하나의 스레드에 문제가 발생하면 전체 프로세스가 영향을 받음

### 멀리 프로세스 대신 멀티 스레드를 사용하는 이유

- (멀티 프로세스 대신 멀티 스레드를 사용하는 것의 의미)
- **프로그램을 여러 개 키는 것보다 하나의 프로그램 안에서 여러 작업을 해결하는 것**

![Untitled](https://s3.us-west-2.amazonaws.com/secure.notion-static.com/2528dd66-4b5b-4c4f-99ec-0ee5796734e2/Untitled.png?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Content-Sha256=UNSIGNED-PAYLOAD&X-Amz-Credential=AKIAT73L2G45EIPT3X45%2F20220110%2Fus-west-2%2Fs3%2Faws4_request&X-Amz-Date=20220110T083203Z&X-Amz-Expires=86400&X-Amz-Signature=b2e83b9de695533b14939b8852e7633928e636717b5f2efd4f1befd3b7136fed&X-Amz-SignedHeaders=host&response-content-disposition=filename%20%3D%22Untitled.png%22&x-id=GetObject)

### 멀티 스레드 장점

- 자원의 효율성 증대
    - 멀티 프로세스로 실행되는 작업을 멀티 스레드로 실행할 경우, **프로세스를 생성하여 자원을 할당하는 시스템 콜이 줄어들어** 자원을 효율적으로 관리
    - 그 이유는 프로세스 간의 Context Switching시 단순히 CPU 레지스터 교체 뿐만 아니라 RAM과 CPU 사이의 캐쉬 메모리에 대한 데이터까지 **초기화되므로 오버헤드가 크기 때문**
    - 스레드는 프로세스 내의 **메모리를 공유**하기 때문에 독립적인 프로세스와 달리 스레드 간 데이터를 주고 받는 것이 간단해지고 시스템 자원 소모가 줄어듦
- 처리 비용 감소 및 응답 시간 단축
    - 프로세스 간의 통신(IPC)보다 스레드 간의 통신의 비용이 적으므로 작업들 간의 통신의 부담이 줄어듦
        
        –> 스레드는 Stack 영역을 제외한 **모든 메모리를 공유하기 때문 (code,data,heap)**
        
    - 프로세스 간의 전환 속도보다 **스레드 간의 전환 속도가 빠름**
    –> Context Switching시 스레드는 Stack 영역만 처리하기 때문
- 주의할 점
    - 동기화 문제
    - 스레드 간의 자원 공유는 전역 변수(데이터 세그먼트)를 이용하므로 함께 상용할 때 충돌이 발생할 수 있음

# NoSQL

### NoSQL이란

- SQL → 데이터를 처리하는 언어
- DBMS의 종류중 하나인 NoSQL
- Not Only SQL, Non-Relational Operational Database SQL로 엇갈리는 의견들이 있음
- 현재 Not Only SQL로 풀어 설명하는 것이 다수
- **Not Only SQL** → 단순히 기존 관계형 DBMS가 갖고 있는 특성뿐만 아니라, 다른 특성들을 **부가적으로 지원**한다는 것을 의미
- NoSQL을 Modern web-scale databases라고 정의하기도 함

### 특징

- 관계형 모델을 사용하지 않으며 테이블간의 조인 기능 없음
- 직접 프로그래밍을 하는 등의 비SQL 인터페이스를 통한 데이터 액세스
- 대부분 여러 대의 데이터베이스 서버를 묶어서(클러스터링) 하나의 데이터베이스를 구성
- 관계형 데이터베이스에서는 지원하는 Data처리 완결성(Transaction ACID 지원) 미보장
- 데이터의 스키마와 속성들을 다양하게 수용 및 동적 정의 (Schema-less)
- 데이터베이스의 중단 없는 서비스와 자동 복구 기능지원
- 다수가 Open Source로 제공
- 확장성, 가용성, 높은 성능

⇒ 초고용량 데이터 처리 등 성능에 특화된 목적을 위해, 비관계형 데이터 저장소에, 비구조적인 데이터를 저장하기 위한 분산 저장 시스템

### 데이터의 구조에(Data Model) 따른 종류

- Key Value DB
    
    **Key와 Value의 쌍으로 데이터가 저장**되는 가장 단순한 형태의 솔루션으로 Amazon의 Dynamo Paper에서 유래되었습니다. Riak, Vodemort, Tokyo 등의 제품이 많이 알려져 있습니다.
    
- Wide Columnar Store
    
    Big Table DB라고도 하며, Google의 BigTable Paper에서 유래되었습니다. **Key Value 에서 발전된 형태의 Column Family 데이터 모델**을 사용하고 있고, HBase, Cassandra, ScyllaDB 등이 이에 해당합니다.
    
- Document DB
    
    Lotus Notes에서 유래되었으며, **JSON, XML과 같은 Collection 데이터 모델 구조**를 채택하고 있습니다. **MongoDB**, CoughDB가 이 종류에 해당합니다.
    
- Graph DB
    
    Euler & Graph Theory에서 유래한 DB입니다. **Nodes, Relationship, Key-Value 데이터 모델**을 채용하고 있습니다. Neo4J, OreientDB 등의 제품이 있습니다.
    

# 참고자료
    
- blocking non blocking sync async
    
    [https://baek-kim-dev.site/38](https://baek-kim-dev.site/38)
    
    [https://velog.io/@codemcd/Sync-VS-Async-Blocking-VS-Non-Blocking-sak6d01fhx](https://velog.io/@codemcd/Sync-VS-Async-Blocking-VS-Non-Blocking-sak6d01fhx)
    
- callback 함수
    
    [https://satisfactoryplace.tistory.com/18](https://satisfactoryplace.tistory.com/18)
    
- 프로세스, 스레드
    
    [https://gmlwjd9405.github.io/2018/09/14/process-vs-thread.html](https://gmlwjd9405.github.io/2018/09/14/process-vs-thread.html)
