```aeris
<const | let> <identifier><: <type>>? <= <initial-value>>
```

```aeris
// const 타입 명시하지 않을 시 다음과 같이 추정
const a: { x: U32 | x == 10 } = 10
const b: { x: I32 | x == -10 } = -10

// let 타입 명시하지 않을 시 다음과 같이 추정 
let c: U32 = 10
let d: I32 = -10
```

변수는 쉐도잉이 가능함
```aeris
const a = 10
const a = "hello"
```
