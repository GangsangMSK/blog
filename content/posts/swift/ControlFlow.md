---
title: "[Swift] ControlFlow(제어문)"
date: 2022-09-27T16:24:19+09:00
draft: true
description: "Swift's Control Flow(if, for, for-in, switch, while etc"
tags: ["Swift"]
categories: ["Swift 문법"]
toc: true
---
## For-In Loops

for-in 반복문은 컬렉션 또는 숫자 범위 내에 있는 목록을 반복한다.

```Swift
for 상수명 in 컬렉션 또는 범위 {
    // 실행될 코드
}
```

'상수명'은 반복문이 돌면서 컬렉션 또는 범위에서 가져온 항목을 담게 될 상수이다.

'컬렉션 또는 범위'는 반복문이 반복되면서 현재의 항목을 참조한다.

문자열 값들의 배열이거나 범위 연산, 문자들로 구성된 문자열일 수 있다.

```Swift
for index in 1...5 {
    print(index)
} // index라는 이름의 상수에 현재 항목이 할당되면서 시작
//1
//2
//3
//4
//5

for _ in 1...5 {
    print("Hello") // _로 참조체 생략 가능
}
//Hello
//Hello
//Hello
//Hello
//Hello

```

***

**아래와 같은 C 스타일의 for문은 Swift 3에서 없어졌다.**
```Swift
for 초기화; 조건식; 증감식 {
    // 실행될 구문
}

for var i = 0; i < 10; i+=1 {  // for i in 0..<10 로 수정해야 함
   print(i)
}  //error: C-style for statement has been removed in Swift 3
```

## 참고자료

[iOS 1주차-9 : 제어문(for-in, while, repeat~while, break, continue, if, guard, switch, where, fallthrough)](https://www.youtube.com/watch?v=3QKVkZj_Pzk&list=PLJqaIeuL7nuEEROQDRcy4XxC9gU6SYYXb&index=11)

[The Swift Programming Language - ControlFlow](https://docs.swift.org/swift-book/LanguageGuide/ControlFlow.html)

[The Swift Programming Language(한국어) - 제어문(ControlFlow)](https://jusung.gitbook.io/the-swift-language-guide/language-guide/05-control-flow#for-in-for-in-loops)