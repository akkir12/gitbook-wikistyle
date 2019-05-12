---
layout: article
title: 파이썬 논리
tags: python
sidebar: null
"​\tnav": layout
mathjax: false
---

# 파이썬 논리값

## 논리값 검사

### 거짓조건

* 거짓으로 정의된 상수 : `None`, `False`
* 모든 숫자들의 영\(0\) : `0` `0.0` `0j` `Decimal(0)` `Fraction(0,1)`
* 빈 시퀀스와 컬렉션 : `''` `()` `[]` `{}` `set()` `range(0)`

  논리값을 돌려주는 연산과 내장 함수는 달리 명시하지 않는 한 항상 거짓의 경우 `0` 이나 `False` 를, 참이면 `1` 이나 `True` 를 돌려줍니다. \(중요한 예외: 논리 연산 `or` 와 `and` 는 항상 피연산자 중 하나를 돌려줍니다.\)

### 논리 연산 -- `and`, `or`, `not`

| 연산 | 결과 |
| :--- | :--- |
| `x or y` | _x_ 가 거짓이면 _y_, 그렇지 않으면 _x_ |
| `x and y` | _x\_가 거짓이면 _x_, 그렇지 않으면 _y_ |
| `not x` | _x_ 가 거짓이면 `True`, 그렇지 않으면 `False` |

* `x or y` : x 가 `false` 일때만 `y` 값을 구함.

  ex\)

  ```python
  x,y = 1,2
  if x==1 or y==2:
  ```

  왼쪽 항이 true 이므로 오른쪽항 계산은 하지않는다.

* `x and y` : x 가 `true` 일때만 `y` 값을 구함.

  ex\)

  ```python
  x,y = 1,2
  if x==2 and y==2:
  ```

  왼쪽 항이 false 이므로 오른쪽항 계산은 하지않는다.

