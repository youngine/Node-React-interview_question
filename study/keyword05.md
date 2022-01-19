# KEYWORD 05
<br>


### 🗝 **[1/17일 STUDY KEYWORD](study/keyword05.md)**
```
EventEmitter, 동기/비동기/블럭/논블럭 api , callback지옥
```

<br>

### * callback이란?
- callback 함수는 다른 함수의 매개변수로 함수를 전달하고, 어떠한 이벤트가 발생한 후 매개변수로 전달한 함수가 다시 호출되는 것
- callback은 쉽게 말하자면 어떤 일을 다른 객체에게 시키고, 그 일이 끝나는 것은 기다리지 않고 끝나고 부를 때까지 다른 일을 하는 것
- 그렇기 때문에 non-block이며, 비동기 방식의 함수를 사용함
<br>

### * callback 함수를 쓰는 이유
- 자바스크립트는 이벤트 중심의 언어이다. 즉, 자바스크립트는 이벤트의 값이 반환될 때까지 기다리지 않고 다음의 이벤트를 계속 실행한다.
- 콜백을 받아야 하는 상황에 callback 함수를 사용하지 않는다면 콜백 함수의 과정이 끝나기 전에 다음 프로세스가 진행될 수 있음.
- 그것을 막고,  차례대로 수행하기 위해 callback 함수를 사용해야함
<br>

### * callback 지옥

```node.js
$.get('http://www.example.org', function(response) {
  task(response, function(result) {
    someTask(result, function(result) {
      someNextTask(result, function(result) {
        someNextNextTask(result, function(result) {
          ...
        })
      })
    })
  });
})
```

- 비동기 처리에 콜백함수를 이용하게 되면 비동기 처리를 중첩시켜서 코드를 작성하기때문에 에러, 예외처리가 어렵고 중첩으로 인한 복잡도가 증가하게 된다.
- 웹서비스를 개발하는 경우 서버에서 데이터를 받아오고 화면에 표시하기까지 수많은 비동기 처리를 하게되면서 위와같은 콜백지옥 현상이 나타나게된다.

<br>

### * promise
- 콜백 함수를 이용한 비동기 처리의 문제점을 해결하기 위해 생겨난 것이 바로 ES6 에서 새로 제안된 Promise.
- 프로미스는 비동기 연산을 감싸는 일종의 프록시 객체

```node.js
function getData() {
  return new Promise((resolve, reject) => {
    $.get('http://www.example.org', function(response) {
      if (response) {
        resolve(response);
      }
      reject(new Error('error'));
    });
  });
}

getData()
  .then(task)
  .then(someTask)
  .then(someNextTask)
  .then(someNextNextTask);
```
<br>

### * async, await
- async, await 은 ES8 부터 자바스크립트에 포함되었고 Promise 를 동기식 코드로 표현할 수 있게 해주는 문법.
- await 을 프로미스 앞에 붙이게 되면 프로미스가 성공했을 때의 결과값이 반환됨

```node.js
async () => {
  const response = await getData();
  const result = await someTask(response);
  const result_2 = await someNextTask(result);
  const result_3 = await someNextNextTask(result_2);
}
```
- 이제 비동기 작업을 감싼 프로미스 API 는 감춰지고 온전히 동기적으로 이해할 수 있는 코드가 만들어짐.
<br>


#### ✅ 참고
1) [node.js의 이벤트루프](https://www.korecmblog.com/node-js-event-loop/#nodejs-event-loop)
2) [callback이란?](https://realrain.net/post/async-await/)
3) [자바스크립트 비동기 처리의 이해](https://hees-dev.tistory.com/33)

<br>
<br>
