```sh
# 빌드 및 실행
docker compose -f `컴포즈 파일 경로` up --build -d

# 중지
docker compose -f `컴포즈 파일 경로` stop

# 중지 & 삭제
docker compose -f `컴포즈 파일 경로` down

# 로그 보기
docker compose -f `컴포즈 파일 경로` logs -f --tail 100
```