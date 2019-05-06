pipeline {
  agent {
    node {
      label 'Start'
    }

  }
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