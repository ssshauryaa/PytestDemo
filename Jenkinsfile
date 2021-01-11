pipeline {
  agent { docker { image 'python:3.8.6' } }
  stages {
    stage('build') {
      steps {
        sh 'pip install -r requirement.txt'
      }
    }
    stage('test') {
      steps {
        sh 'pytest'
      }   
    }
  }
}