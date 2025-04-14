```aeris
<const | let> <identifier><: <type>>? <= <initial-value>>
```

```aeris
// premise 문법은 추후 수정 & 구체화 예정

// const 타입 명시하지 않을 시 다음과 같이 추정
const a: U32 & premise {this==10} = 10
const b: I32 & premise {this==-10} = -10

// let 타입 명시하지 않을 시 다음과 같이 추정 
let c: U32 = 10
let d: I32 = -10
```
