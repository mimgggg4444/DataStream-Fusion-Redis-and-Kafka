
### 요구사항 정의
- 자사 proj의 경우 합의, 요구사항 내용 회의내에서 논의 결정 -> 명시/문서화로 정확한 상호컨펌

  구분, 서비스(메뉴), 필요기능, 기능설명, 레퍼런스, 우선순위


1. 이서비스 왜 개발?
     1. 영향범위 파악, 확장성 고려
2. 이 서비스 런칭 시점
     1. 개발 우선순위 완성도 영향
3. 자원 확보
     1. 일을 하기 위해 필요한 도구
4. 이 서비스 주요 클라이언트
     1. 요구사항 합의, 개발 현황 공유, client test, 런칭후 모니터링, 장애 공유
  

간단한 요구사항 정의 - TEST
- 서비스명: 특정상품최저가
- 서비스 요구사항 정의:
    1. 요구사항 명: 최저가 반환
    2. 요구사항 설명:
    3. 중요도:
-> 키워드로 상품검색, 중복없는 배송비 포함 최저가 10개 전달


 ---
 ---

### 품질 요건 = 해당 서비스가 갖추어야 하는 기능적, 기술적 요건
- 가용성 rto rpo 장애 uptime
    1. 다운 발생시 정상화 방안, 목표시간
  
- 성능 ops/sec/tps/datain/s, dataout/s
- 비용
- 보안
- 효율성

### 가격비교 서비스의 품질요건 <예시>
- 가용성 99.95(4.38)
- 성능용량 200ops/sec 20tps ->계산방법
- 비용 h/w, s/w의 비용
- 보안 내부망
- 효율성 api rest, swagger 명세서 apigeteway


---
---
### data
keyword > prodgrpld > prodld


### 논리적 흐름
1. api get request
2. keyword조회
3. keyword prodgrpld
4. prodgrpld{prodld.price}
5. api get response

---
1. 타 서비스 최저가 서비스 호출 keyword
2. keyword: {prodgrpld... } 조회
3. redis에 없으면 elasticsearch조회 prodgrpld조회 후 redis에 저장
4. prodgrpld 데이터 조회
5. 없다면 3과 똑같이 















---
---

