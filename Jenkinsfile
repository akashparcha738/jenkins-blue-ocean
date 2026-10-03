pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'pwd date'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'test step'
          }
        }

        stage('Test para') {
          steps {
            echo 'test para'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'deploy'
        sleep 10
      }
    }

  }
}