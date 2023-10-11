pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'whoami' // 현재 사용자 확인
        sh 'pwd' // 현재 작업 디렉토리 위치 확인
        sh './gradlew clean build'
      }
    }

  }
}