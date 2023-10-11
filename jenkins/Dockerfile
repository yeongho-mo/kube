FROM openjdk:17-alpine
EXPOSE 8006

ARG JAR_FILE=build/libs/*.jar # 빌드된 Jar 파일

# JAR_FILE의 경로 출력
RUN echo "$(pwd)"
RUN echo "JAR_FILE 경로: ${JAR_FILE}"

COPY ${JAR_FILE} deploy-app.jar # deploy-app.jar 파일명으로 복사
CMD java -jar ./deploy-app.jar # jar 파일 실행


