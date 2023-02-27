# 알림창 만들기 (alert) - UIAlertController, UIAlertAction

앱을 사용하다 보면 이러한 창을 많이 볼수 있습니다.

오늘은 간단하게 알림창을 띄우는 방법을 알아보겠습니다.

<img width="249" alt="스크린샷 2023-02-27 오전 11 35 51" src="https://user-images.githubusercontent.com/124115721/221460143-106592bc-ed0f-4cc8-baa1-284a83068f6a.png">

우선 알림창에 들어갈 내용을 작성해 주세요
```swift
//1. 알림창 내용 작성
let alert = UIAlertController(title: "압력 불가", message: "값을 확인해 주세요", preferredStyle: .alert)
```

다음으로 버튼을 만들어 줍니다.
```swift
//2. 확인 버튼 만들기
let confirm = UIAlertAction(title: "확인", style: .default, handler: nil) 
// handler는 만든 확인 버튼을 눌렀을 때 특정 동작을 추가할 수 있습니다.
```

만든 확인 버튼을 알림창에 추가해 줍니다.
```swift
//3. 만든 버튼을 알림창에 추가하기
alert.addAction(confirm)
```

완성된 알림창을 ViewController에 보여줍니다.
```swift
present(alert,animated: true,completion: nil) 
// completion는 present가 끝난 후 보여줄 동작

```


추가로 같은 알림창을 여러번 사용해야 한다면 기능 함수를 만들어 사용할 수도 있습니다.

```swift
func warming() {
    //1. 알림창 내용 작성
    let alert = UIAlertController(title:"압력 불가", message: "값을 확인해 주세요", preferredStyle: .alert)

    //2. 확인 버튼 만들기
    let confirm = UIAlertAction(title: "확인", style: .default, handler: nil)

    //3. 만든 버튼을 알림창에 추가하기
    alert.addAction(confirm)

    //4. 경고창 보이기
    present(alert,animated: true,completion: nil)
}

// ViewController 버튼에 연결
@IBAction func button(_ sender: Any) {
    warming()
}

```
ViewController에 연결되어있는 버튼을 눌었을 때 아래와 같은 창을 확인할 수 있습니다.

<img width="249" alt="스크린샷 2023-02-27 오전 11 35 51" src="https://user-images.githubusercontent.com/124115721/221460143-106592bc-ed0f-4cc8-baa1-284a83068f6a.png">
