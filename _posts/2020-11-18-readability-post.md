---
layout: post
title: "파이썬 - 영어로 된 문장을 입력하여 대문자와 소문자가 나온 횟수 구하기"
date: 2020-11-17
excerpt: "Python Algorithm"
tags: [sample post, readability, test]
comments: true
---

## 파이썬 - 영어로 된 문장을 입력하여 대문자와 소문자가 나온 횟수 구하기

안녕하세요. 오늘은 파이썬에서 영어로 된 문장을 입력받아 대문자와 소문자가 나온 횟수를 구해보는 코드를 작성해보겠습니다.
그럼 바로 문제를 살펴보도록 할게요.


### 문제 

* 영어로 된 문장을 입력하여 대문자와 소문자가 나온 횟수을 구하는 코드를 작성하세요.
* Tip. 아스키코드 (인터넷 검색)
* ord()라는 함수 사용하기.


### 출력 화면

영어로 된 문장을 입력하세요:swHAcaDemY
대문자 수 : 4
소문자 수 : 6


---

## 코드
a = input("영어로 된 문장을 입력하세요:")
b = []
c = []
d = 0
while d < len(a):
    if ord(a[d]) >= 65 and ord(a[d]) <= 90:
        b += a[d]
    if ord(a[d]) >= 97 and ord(a[d]) <= 122:
        c += a[d]
    d += 1
print(b)
print("대문자 수 :",len(b))
print("소문자 수 :",len(c))
---

