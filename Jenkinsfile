pipeline {
  agent {
    docker {
      image 'maven:3-alpine'
      args '-v /root/.m2:/root/.m2'
    }

  }
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'mvn -B -DskipTests clean package'
          }
        }
        stage('Build-p') {
          steps {
            sh 'echo "hello"'
          }
        }
      }
    }
    stage('LastStep') {
      steps {
        sh 'echo "done"'
      }
    }
  }
}