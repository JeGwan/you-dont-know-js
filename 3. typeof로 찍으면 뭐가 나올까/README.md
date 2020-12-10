## Q

typeof로 다음과 같은 녀석들을 찍으면 뭐가나올까?

- string
- boolean
- number
- undefined
- null
- new Symbol()
- object (그냥 {})
- function
- array (그냥 [])

## A

- string => "string"
- boolean => "boolean"
- number => "number"
- undefined => "undefined"
- null => "object"
- new Symbol() => "symbol"
- object (그냥 {}) => "object"
- function => "function"
- array (그냥 []) => "object"

다른 건 예상대로 나왔는데 두놈이 이상하다

null 은 object로 나온다.
function은 object의 하위 타입인데 function 이라 나온다.

자바스크립트의 데이터타입은 원시타입(스불넘언널심) + 오브젝트 뿐이다.
근데 저 두놈만 타입그대로를 안뱉는다...!
