pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'i want to build'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'i want to test'
          }
        }

        stage('Deploy') {
          steps {
            echo 'deployed'
          }
        }

      }
    }

  }
}