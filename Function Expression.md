##  :star:Named Function Expression (기명 함수 표현식)

```html
const sayHi = function() {
console.log('Hi');
};

console.log(sayHi.name); //sayHi
```
이름이 없는 함수에 변수 할당할 때는 변수의 name속성은 변수 이름 그자체를 문자열로 가짐
```html
const sayHi = function printHiInConsole() {
console.log('Hi');
};

console.log(sayHi.name); //printHiInConsole
```
함수에 이름 붙여주게 되면 name속성은 함수 이름을 문자열로 갖게 됨
```html
const sayHi = function printHiInConsole() {
console.log('Hi');
};
printHiInConsole(); //ReferebceError
```
이 함수 이름은 내부에서 함수 자체를 가리킬 때 사용할 수 있고 함수를 외부에서 호출할떄 사용
할 수 없음
```html
let countdown = function printCountdown(n) {
  console.log(n);
  if (n === 0) {
    console.log('End!');
  } else {
    printCountdown(n - 1);
  }
};

let myFunction = countdown;

countdown = null;

myFunction(5);
```

## :star:즉시 실행 함수
함수 선언과 동시에 즉시 실행되는 함수= 즉시 실행 함수 (표현)<br>
 * Immediately Invoked Function Expression, 줄여서 IIFE <br>
```html
(function () {
  console.log('Hi!');
})();

(function sayHi() {
  console.log('Hi!');
})();

sayHi(); // ReferenceError

```
> 함수에 이름지어도 외부에서 사용 불가능<br>
 프로그램 초기화 기능에 많이 활용

