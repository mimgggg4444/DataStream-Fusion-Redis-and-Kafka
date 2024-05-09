### 가격비교 rest api 기본틀 개발

rest api 기본틀

browser - view(jsp) - controller(controller) - model(service, repo) - data(sql, nosql)

장 - 분리, 확장 / 단 - view - model 의존성


### 가격비교 api redis lib 종류 선택

jedis - 개발 복잡도 낮다

letture - 다양한 옵션, scaling에 좋음, non blocking reactive application 유리


### 가격정보데이터 datatype 분할

redis data type

- string 1:1
- lists 순서(queue, stack)
- sets 순서 상관없이 저장, 중복 불가
- sorted sets 
- hashes
- 
- zadd 입력
- zcard count
- zrange 정렬순서로조회
- zrangebyscore score로 함께 조회
- zrem 삭제
- zscore 특정 member score조회
- zrank 특정 member rank조회



