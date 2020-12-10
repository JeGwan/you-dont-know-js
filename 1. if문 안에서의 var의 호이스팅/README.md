## Q

정말 if문 안에서 var를 써도 글로벌 스코프로 호이스팅 될까?

## A

된다. if 조건문이 false여서 접근을 못하는 경우에도 해당 스코프 안에서 var 라 선언된 변수는 호이스팅이 되버린다!

따라서 polyfill 을 만들 경우 가능한 if 문 안에서 var 로 선언하지 말고 그냥 변수에 할당하는 듯이 해야한다

```js
if (typeof myPolyfill === "undefined") {
  myPolyfill = "someThing";
}
```
