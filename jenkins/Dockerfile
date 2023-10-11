FROM openjdk:17-alpine
EXPOSE 8006

# 컨테이너 내의 작업 디렉토리 설정
WORKDIR /app

# JAR 파일을 컨테이너로 복사
COPY /var/lib/jenkins/workspace/test1_main/build/libs/jenkinsTest-0.0.1-SNAPSHOT.jar .

# JAR 파일을 실행
CMD ["java", "-jar", "jenkinsTest-0.0.1-SNAPSHOT.jar"]

