## Q

```js
const a = 1 / "a"; // NaN
console.log(a); // NaN
console.log(NaN === a); // false
console.log(NaN === NaN); // false
console.log(Number.isNaN(a)); // true
console.log(Number.isNaN("a")); // false
```

## A

NaN 은 NaN 끼리 동일하지 않다...!
그래서 stric equal 연산자로 비교할 수가 없다!
따라서 NaN 을 확인하려면 Number의 프로토타입 메소드 .isNaN 를 써야한다.
