pipeline {
  agent any
  stages {
    stage('Start-Build') {
      steps {
        echo 'Build Start'
      }
    }
    stage('Test-Stage-1') {
      parallel {
        stage('Test-Stage-1') {
          steps {
            build 'MAVEN_D4'
          }
        }
        stage('Test-Stage-2') {
          steps {
            echo 'Stage 2'
          }
        }
      }
    }
    stage('Test-Stage-3') {
      steps {
        echo 'Third Job'
      }
    }
  }
}