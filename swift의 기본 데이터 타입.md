# swift의 기본 데이터 타입
## Int
64bit의 정수 타입
```swift
var someInt: Int = 10 // 10
someInt: Int = -5 // -5
someInt = 5.5 // error
```

## UInt
64bit의 양의 정수 타입
```swi
var someUInt: UInt = 10 // 10
someUInt = -5 // error
someUInt = 5.5 // error
```

## Flot
32bit의 실수 타입
```swift
var someFloat = 10 // 10.0
someFloat = -5 // -5.0
someFloat = 5.5 // 5.5
```

## Double
64bit의 실수 타입
```swift
var someDoublet: Double = 10 // 10.0
someDoublet = -5 // -5.0
someDoublet = 5.5 // 5.5
```

## Character
하나의 문자만 올 수 있는 문자 타입
```swift
var someCharacter: Character = "A" // A
someCharacter = "ABC" // error
```

## String
여러 문자가 올 수 있는 문자열 타입
```swift
var someString: String = "ABCD" // ABCD
someString = "A" // A
```

## Bool
true와 false만 가지는 타입
```swift
var someBool: Bool = true // true
someBool = false // false
someBool = 5 // error
```

## Any
모든 타입을 가질 수 있는 타입
```swift
var someAny: Any = "12ABC" // 12ABC
someAny = 12345 // 12345
someAny = 10.5 // 10.5
```
