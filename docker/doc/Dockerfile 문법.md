```Dockerfile

# 베이스 이미지 선택
FROM 이미지명:태그 

# 라벨링
LABEL `원하는 키`=`원하는 값`

# "빌드" 할 때 실행되는 명령어, 레이어를 생성한다
RUN `원하는 명령어`
```

# 목표
- 우분투 베이스 이미지
- nginx 설치
- html 하나 올려서
- 서버 기동