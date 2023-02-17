# truncatingRemainder(dividingBy:) 메서드

계산기를 만들다 알게 된 truncatingRemainder(dividingBy:) 메서드를 알아보고자 한다.

Int 타입에서 나머지 값을 구하기 위해 %(나머지 연산자)를 사용한다.
```swift
5 % 2 // 1
6 % 2 // 0
```

만약 소수점이 있는 Double, Float의 경우 나머지값을 구하려면 truncatingRemainder(dividingBy:) 메서드를 사용해야 한다.
```swift
let a = 5.0
a.truncatingRemainder(dividingBy: 2) // 1
let b = 6.0
b.truncatingRemainder(dividingBy: 2) // 0

//숫자를 바로 넣어 사용 가능
5.0.truncatingRemainder(dividingBy: 2) // 1
```
