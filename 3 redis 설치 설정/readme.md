### 


1. aws
2. 회원가입

3. ec2
4. ubuntu os
5. instants - t2 micro

6. 키 페어 설정

7. 보안그룹생성
8. 위치무관
9. 8gb gp2

10. 인스턴스 연결 -> 연결

---
명령어

11. sudo su
12. apt-get update
13. apt-get install redis-server -> y -> service redis status
14. cd etc/redis
15. ps -ef | grep redis // port번호 확인

16. redis-cli -> info

---
---

### redis configuration

- redis 
- vmname : first(master) <---sync---> second (replica)
- sentinel은 홀수개로 설치



1. aws에서 이미지 생성 -> 인스턴스에서 선택후 작업 클릭
   1. image for second redis
  
2. 왼쪽 이미지 ami 에서 확인 가능

3. redis-cli
   1. repliceof (인스턴스의 ipv4 입력하기) 6379(check port number)
  
4. info를 통해서 확인

5. instants 에서 보안
   1. 인바운드 규칙 반환
   2. 규칙추가 사용자지정 tcp 6379
   3. launch (sg-05bcecf ... ) 설정
   4. 저장
  
6. tail -f /var/log/redis/redis-server.log - sync확인

7. redis cli info

8. first, second 들어가서 연결되었는지 확인.

9. set min rediskafkalecture

10. replica에서 다시 확인
    1. get min
   
11. 레플리카에서 설정
    1. config set maxmemory 500mb
   
12. config get maxmemory

---
---


### ServerSentinel 설치














