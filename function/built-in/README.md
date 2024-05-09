# Mysql note - Function - built-in (내장 함수)

몰랐던 내장함수 정리

## Table of Contents

- [내장함수란?](#내장함수란?)
- [LEAST](#LEAST)
- [GREATEST](#GREATEST)

## 내장함수란?

- Mysql 자체에서 구현되있는 함수를 말한다. (built-in)
- 숫자, 문자, 논리, 집계, 날짜 등의 데이터에서 유의미한 값을 도출하는데 쓰인다.

## LEAST

- 여러 값 중, 최소값을 구하는 함수.
- 2개 이상의 파라미터를 넣을 수 있다.
```SQL
SELECT LEAST(10, 20) -- 결과: 10
SELECT LEAST(10, 20, 5) -- 결과: 5
```
- 숫자뿐만 아니라 문자도 가능하다.
```SQL
SELECT LEAST('a', 'b') -- 결과: a
SELECT LEAST('a', 'b', 'c') -- 결과: a
SELECT LEAST('a', 'b', 'c', null) -- 결과: null
```

## GREATEST
- 여러 값 중, 최대값을 구하는 함수.
- 2개 이상의 파라미터를 넣을 수 있다.
```SQL
SELECT GREATEST(10, 20) -- 결과: 20
SELECT GREATEST(10, 20, 5) -- 결과: 20
```
- 숫자뿐만 아니라 문자도 가능하다.
```SQL
SELECT GREATEST('a', 'b') -- 결과: b
SELECT GREATEST('a', 'b', 'c') -- 결과: c
SELECT GREATEST('a', 'b', 'c', null) -- 결과: c
```