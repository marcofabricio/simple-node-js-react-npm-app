pipeline {
  agent {
    docker {
      image 'node:6-alpine'
      args '-p 3000:3000'
    }

  }
  stages {
    stage('teste') {
      steps {
        build 'teste'
        fileExists 'teste'
      }
    }
    stage('tetete') {
      steps {
        sh 'echo "tete"'
      }
    }
  }
  environment {
    branch = 'master'
  }
}