pipeline {
  agent none
  stages {
    stage('PWD') {
      steps {
        sh 'pwd'
      }
    }
    stage('DIR INTO') {
      steps {
        dir(path: 'src') {
          sh 'pwd'
        }

      }
    }
  }
}