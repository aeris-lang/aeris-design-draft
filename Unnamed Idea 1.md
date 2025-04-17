concept 1
```aeris
let a: U32 ?x x in 0..100 = 10
```

concept 2
```aeris
let a: { x: U32 | x in 0..100 } = 10
```

concept 3
```aeris
let a: U32:x x in 0..100 = 10
```

concept 4
```aeris
let a: U32
premise a in 0..100
a = 10
```