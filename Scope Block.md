코드블록 내에서 상위 스코프에서 내부 값에 접근 불가한 격리된 스코프를 생성할 수 있음
```aeris
const a = 10
(
	const b = 20
	println a // compile success
)

println b // compile error
```

스코프 블록은 표현식으로서 취급됨: 반환값을 가질 수 있음
```aeris
const bar = (
	const foo = getFoo()
	if foo.isSomething() return // 명시적 반환
	foo.bar() // 암묵적 반환
)
```
