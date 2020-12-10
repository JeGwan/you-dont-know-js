## Q

```js
const a = [1, 2, 3];
delete a[1];
console.log(a);
a.forEach((element) => console.log(element));
```

배열을 선언해놓고 지우면, 뭐가 뜰까?

## A

배열도 객체이기 때문에 숫자를 키로 가지고 있던 1이란 놈은 사라진다.
다만 그렇게 사라져도 length 프로퍼티는 변하지 않는다.
근데 forEach로 돌리면 length가 줄어든 것처럼 지운놈은 건너뛰고 돌아버린다.

참.. 언어 \*같다.
