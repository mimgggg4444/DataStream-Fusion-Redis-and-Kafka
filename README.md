# test-using-database


mysql

mongodb

oracle database

redis

postgresql

firestore

mysql - 정해진 스키마에 따라 데이터를 테이블

nosql - 스키마가 없거나 유연한 스키마



디스크베이스 - 영구 저장 / 나머지 / 쿼리 최적화

인메모리 - 빠름 / 실시간 / redis / volatility(휘발성)


- Redis - https://github.com/microsoftarchive/redis/releases
- Redis Insight - https://redis.io/insight/
- Hedisql - https://www.heidisql.com/download.php (윈도우 전용)
- mysql - https://velog.io/@heiswicked/M1%EC%97%90%EC%84%9C-MySQL-%EC%84%A4%EC%B9%98brew%EB%A1%9C

```
CREATE TABLE `user` (
	`id` BIGINT(19) NOT NULL AUTO_INCREMENT,
	`username` VARCHAR(50) NOT NULL DEFAULT '' COLLATE 'utf8mb4_0900_ai_ci',
	`password` VARCHAR(50) NOT NULL DEFAULT '' COLLATE 'utf8mb4_0900_ai_ci',
	PRIMARY KEY (`id`) USING BTREE
)
COLLATE='utf8mb4_0900_ai_ci'
ENGINE=InnoDB
;

```



### join에 관한 설명


### redis

쉽고 편한 redis


---
---



