### `user README.md`

#### `judy-community-backend-user`

# Judy Community User Backend

사용자 프로필 및 관련 작업을 관리하는 백엔드 서비스입니다.

## 구조

```
judy-community-backend-user/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/
│   │   │       └── judycorp/
│   │   │           └── user/
│   │   │               ├── config/
│   │   │               ├── controller/
│   │   │               ├── dto/
│   │   │               ├── entity/
│   │   │               ├── exception/
│   │   │               ├── repository/
│   │   │               ├── service/
│   │   │               └── ApplicationUser.java
│   ├── resources/
│   │   └── application.properties
├── Dockerfile
├── build.gradle.kts
└── settings.gradle.kts
└── .github/
    └── workflows/
        └── ci-cd.yml
```

## 기능

- 사용자 프로필 조회
- 사용자 프로필 수정
- 사용자 정보 관리

## 설치 및 실행

### 사전 요구 사항

- [Docker](https://www.docker.com/get-started)
- [JDK 17](https://adoptopenjdk.net/)

### Docker 이미지 빌드 및 실행

```bash
./gradlew build
docker build -t your_dockerhub_username/judy-community-backend-user .
docker run -p 8082:8080 your_dockerhub_username/judy-community-backend-user
```
