## Spring boot 를 이용한 jwt 인증 구현
### spring boot / spring security / jpa / h2-database 

```
JWT 장점: 
- 중앙의 인증서버, 데이터 스토어에 대한 의존성 없음, 시스템 수평 확장 유리
- Base64 URL Safe Encoding -> URL, Cookie, Header 모두 사용 가능

JWT 단점:
- Payload의 정보가 많아지면 네트워크 사용량 증가, 데이터 설계 고려 필요
- 토큰이 클라이언트에 저장, 서버에서 클라이언트의 토큰을 조작할 수 없음
```

1. 첫 번째  
:o:401 unauthorized 해결을 위한 Securuity 설정  
:o:Datasource, JPA 설정  
:o:Entity 생성  
:o:H2 consle 결과 확인 
  
2. 두 번째  
:o:jwt 설정 추가  
:o:jwt 관련 코드 개발  
:o:Security 설정 추가  

3. 세 번째  
:o:외부와의 통신에 사용할 DTO 클래스 생성  
:o:Repository 관련 코드 생성  
:o:로그인 API, 관련 로직 생성  

4. 네 번째  
:o:회원가입 API 생성  
:o:권한 검증 확인  