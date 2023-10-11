FROM openjdk:17-alpine
EXPOSE 8006

ARG JAR_FILE=build/libs/*.jar # 빌드된 Jar 파일

COPY ${JAR_FILE} deploy-app.jar # deploy-app.jar 파일명으로 복사
CMD java -jar ./deploy-app.jar # jar 파일 실행


