```aeris
premise <premise: Bool>
```

premise 선언으로 코드 단위의 전제를 요구할 수 있음
```aeris
func foo a: U32 =Frac {
	premise a != 0
	100 / a
}

func main {
	println foo 20 // 5
	println foo 0 // compile error
}
```
