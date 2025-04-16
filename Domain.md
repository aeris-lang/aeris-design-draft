정의역
타입으로서 작동함
```aeris
const a: { x: U32 | 0 < x <= 100 } = 10
// 이 코드에선 큰 의미없음: a는 항상 10으로서 취급됨
```

```aeris
let a: { x: U32 | 0 < x <= 100 } = 10
a = 101 // compile error
```

