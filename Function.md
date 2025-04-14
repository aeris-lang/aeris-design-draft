```aeris
func <name> <<arg> <: <arg-type>>?>? <= <return-type>>? {
	<body>
}
```
함수는 0 또는 1개의 매개변수를 가질 수 있음

```aeris
func foo {

}

func bar =Void {

}
```
반환 타입 생략 시 기본적으로 Void 타입

```aeris
func foo num: I32 {
	
}

func bar {

}

func main {
	foo 10 // foo 호출
	bar // bar 호출
}
```

```aeris
func foo values: (UI32, UI32) {

}

func main {
	foo (10, 20)
}
```
튜플 타입을 받는 함수

```aeris
func foo (a: UI32, b: UI32) {

}
```
구조 분해 할당 + 타입 생략(컴파일러가 자동으로 추정)
