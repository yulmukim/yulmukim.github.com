---
layout: post
title: "[파이썬 프로그래밍] 영어로 된 문장을 입력하여 대문자와 소문자가 나온 횟수 구하기"
date: 2020-11-17
excerpt: "Python Algorithm"
tags: [sample post, readability, test]
comments: true
---

## [파이썬 프로그래밍] 영어로 된 문장을 입력하여 대문자와 소문자가 나온 횟수 구하기

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


### 문제 해결 과정

https://www.google.com/imgres?imgurl=https%3A%2F%2Ft1.daumcdn.net%2Fcfile%2Ftistory%2F2108CF3D535B217E17&imgrefurl=https%3A%2F%2Fenter.tistory.com%2F49&tbnid=9i6wzy7dJcVM-M&vet=12ahUKEwj2tcfg-YntAhX-zYsBHQdtCbcQMygBegUIARCiAQ..i&docid=rYEtWo-0Mho8dM&w=488&h=717&q=%EC%95%84%EC%8A%A4%ED%82%A4%EC%BD%94%EB%93%9C%20%EB%8C%80%EC%86%8C%EB%AC%B8%EC%9E%90&ved=2ahUKEwj2tcfg-YntAhX-zYsBHQdtCbcQMygBegUIARCiAQ
https://www.google.com/imgres?imgurl=https%3A%2F%2Ft1.daumcdn.net%2Fcfile%2Ftistory%2F2108CF3D535B217E17&imgrefurl=https%3A%2F%2Fenter.tistory.com%2F49&tbnid=9i6wzy7dJcVM-M&vet=12ahUKEwj2tcfg-YntAhX-zYsBHQdtCbcQMygBegUIARCiAQ..i&docid=rYEtWo-0Mho8dM&w=488&h=717&q=%EC%95%84%EC%8A%A4%ED%82%A4%EC%BD%94%EB%93%9C%20%EB%8C%80%EC%86%8C%EB%AC%B8%EC%9E%90&ved=2ahUKEwj2tcfg-YntAhX-zYsBHQdtCbcQMygBegUIARCiAQ

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

