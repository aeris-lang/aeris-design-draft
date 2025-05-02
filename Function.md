TODO: 문법 모호함. 개선 필요

```aeris
func <name> <= <return-type>>? {
	<body>
}
```

```aeris
func foo {

}

func bar =<> {

}
```
반환 타입 생략 시 기본적으로 () 타입

```aeris
func foo a: I32 b: I32 {
	a + b
}

func bar {

}

func main {
	foo 10 20 // foo 호출
	bar // bar 호출
	foo 10
		20
	
}
```

```aeris
```


```aeris
func foo values: <UI32, UI32> {

}

func main {
	foo <10, 20>
}
```
튜플 타입을 받는 함수

```aeris
func foo <a: UI32, b: UI32> {

}
```
구조 분해 할당 + 타입 생략(컴파일러가 자동으로 추정)

#### 오버로딩
```aeris
func foo a: I32 =I32 {
	a^2 + 2*a + 3
}

func foo s: String {
	println "{s} Hello, World!"
}
```

```aeris
func foo a: I32 {

}

// compile error
func foo a: I32 b: I32 {

}
```
매개변수 개수 다를 수 없음

```aeris
func foo a: I32 {

}

// compile success
func foo <a: I32 b: I32> {

}
```
