---
title: Database Keyword
date: 2021-02-02 08:57:00 +0900
categories: [Keywords]
tags: [database]     # TAG names should always be lowercase
---

# 기본 기능

- 검색
- 갱신
  - 등록
  - 수정
  - 제거
  - 고유성

- 동시성 제어
- 장애 대응
  - 데이터 다중화
  - 백업

- 보안

# 종류

- 계층형 데이터베이스
- 관계형 데이터베이스
- 객체지향 데이터베이스와 XML 데이터베이스
- NoSQL 데이터베이스

# 관계형 데이터베이스

- SQL
- 테이블
- 행과 열


# DB 서버 다중화

- Active-Active
- Active-Stanby
  - Cold-Stanby
  - Hot-Stanby

- 리플리케이션
- Shared Disk
- Shared Nothing (Sharding)

# SQL

## Data Definition Language

- CREATE
- DROP
- ALTER

## Data Manipulation Language

- SELECT
- INSERT
- UPDATE
- DELETE

## Data Control Language

- COMMIT
- ROLLBACK

# Transaction

- Atomic
- Consistency
- Isolation
  - Read Uncommitted
  - Read Committed
  - Repeatable Read
  - Serializable
- Durability

- Lock Timeout
- Deadlock

# 테이블 설계

테이블은 기본키 집합을 열의 집합과 연결하는 함수

- 정규형
  - 함수 종속성
    - 제1정규형
      - 릴레이션이어야 할 것
    - 제2정규형
      - 후보키의 진부분집합 -> 키가 아닌 속성
    - 제3정규형
      - 키가 아닌 속성 -> 키가 아닌 속성
    - BCNF
      - 키가 아닌 속성 -> 후보키의 진부분집합
  - 결합 종속성
    - 무손실 분해를 할 수 있는 상태
    - 제4정규형
    - 제5정규형

# 릴레이션의 직교성
- 중복을 해결해 얻는 이점
  - 변칙을 막을 수 있다.
  - 필요한 데이터가 어디에 있는지 명확해진다.
  - 쿼리의 작성이 선언적이 된다.
  - 불필요한 무손실 분해는 필요 없다.

# 백업

- WAL (디스크)
- 데이터베이스 버퍼 (메모리)
- 데이터베이스 파일 (디스크)

- 핫 백업, 콜드 백업
- 논리 백업, 물리 백업
- 풀 백업, 부분 백업 (증분/차등)

# 성능

- Index
  - B-Tree
    - MySQL은 기본적으로 B+Tree
- Optimizer
- Execution Plan

# 관계형 모델

- 집합론에 기인하는 데이터 모델
- 릴레이션 단위로 다양한 연산을 사용해 질의를 수행하는 데이터 모델

- Relation
  - Table
  - Heading
    - a set of Attributes
  - Body
    - a set of Tuples

## 연산의 종류

- Restrict
- Projection
- Extend
- Rename
- Union
- Intersect
- Difference
- Product
- Join

- 연산의 결과는 릴레이션 -> Closure 성질

## 데이터 형식

- Domain