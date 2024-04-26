# Mysql note - User Privileges

사용자 권한 설정

## Table of Contents

- [User Privileges란?](#User&nbsp;Privileges란?)
- [목적](#목적)
- [쓰임새](#쓰임새)

## User Privileges란?

- 데이터베이스에 접근할 수 있는 사용자들에게 데이터베이스 및 테이블을 한정하여 여러 권한을 주는 기능
- 여러 권한
    - CREATE, ALTER, DROP 같은 테이블 생성, 변경, 삭제 권한
    - INSERT, SELECT, UPDATE, DELETE 등의 테이블 레코드 관련 권한
    - EXECUTE, CREATE ROUTINE 등의 프로시저 관련 권한

## 목적

- 사용자마다 데이터베이스 접근에 제한을 두어 보안 강화
- 데이터베이스 접근 제한을 넘어 여러 명령어 제한을 통한 쿼리 실수 방지

## 쓰임새

- 데이터베이스에 접근하는 개발자들에게 용도에 맞는 사용자 아이디를 건네주자
    - 예)주니어 개발자: 테이블 생성 및 삭제 권한을 주지 않고, 특정 테이블의 SELECT 권한만 주기

