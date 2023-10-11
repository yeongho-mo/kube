pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'chmod +x ./gradlew'
        sh './gradlew clean build'
      }
    }

    stage('docker build') {
      steps {
        script {
          // Docker 빌드 단계
          def imageName = 'test-docker-image' // 이미지 이름 설정
          def dockerfile = 'Dockerfile' // 도커파일 이름 (현재 디렉토리에 있음)

          echo pwd

          // Docker 이미지 빌드
          sh "docker build -t $imageName -f $dockerfile ."

          // Docker 이미지를 원격 레지스트리에 푸시 (선택적)
           echo "docker push $imageName 도커이미지 푸쉬"
        }
      }
    }
  }
}