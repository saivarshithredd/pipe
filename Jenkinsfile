pipeline {
  agent any
  stages {
    stage('build') {
      steps {
         script {
            docker.build('app')
        }
      }
    }
    stage('run') {
      steps {
        script {
           bat 'docker run app'
        }
      }
    }
  }
}
