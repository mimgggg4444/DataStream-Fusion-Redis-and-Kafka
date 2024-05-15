### 보안

정상적인 입력: "Alice"
SQL 인젝션 시도: "Alice'; DROP TABLE users; --"


# SQL 쿼리 생성 (SQL 인젝션 취약점이 있는 부분)
query = "SELECT * FROM users WHERE username = '{}' AND password = '{}'".format(username, password)

정상적인 로그인: user1, password1
SQL 인젝션 시도: user1' OR '1'='1'; --, password1



# SQL 쿼리 생성 (SQL 인젝션 취약점이 있는 부분)
query = "SELECT * FROM users WHERE username = '{}'".format(user_input)


데이터베이스를 완전히 삭제
'; DROP DATABASE dbname; --


