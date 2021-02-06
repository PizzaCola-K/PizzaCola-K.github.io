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
  - 제1정규형
  - 제2정규형
  - 제3정규형
  - 제4정규형
  - 제5정규형

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
