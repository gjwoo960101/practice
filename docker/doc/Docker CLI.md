
```bash
# 이미지 목록 확인
docker images

# 컨테이너 목록 확인
docker ps -a

# 이미지 가져오기
docker pull `이미지 주소:태그`

# 이미지 삭제하기
docker rmi `이미지명:태그` 혹은 `이미지 아이디`

# 이미지 빌드
docker build \
    -t '이미지명:태그' \
    `도커파일 경로`

# 이미지 -> 컨테이너 생성
docker create \
    # # 포트포워딩
    # -p 
    # # 볼륨 마운팅
    # -v
    # 컨테이너 명 설정
    --name 컨테이너명\
    이미지명:이미지태그

# 컨테이너 삭제(실행중인 건 안 됨)
docker rm 컨테이너명
    

# 컨테이너 실행
docker start 컨테이너명

# 컨테이너 중지
docker stop 컨테이너명

# 컨테이너 재시작
docker restart 컨테이너명

# 동작중인 컨테이너 내부로 명령을 전달
docker exec '컨테이너명' '명렁어'

# 컨테이너 내부로 진입
# docker exec -it test /bin/bash
docker exec -it '컨테이너명' 'CLI 툴'

```

1. 컨테이너 내부로 진입
2. nginx를 설치
3. nginx 실행