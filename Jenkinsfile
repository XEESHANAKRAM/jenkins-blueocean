pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'pwd'
        echo 'Hello'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            sleep 10
            echo 'Test Success'
          }
        }

        stage('Success') {
          steps {
            echo 'Success'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy code'
      }
    }

    stage('Deploy on Server') {
      steps {
        echo 'Tested'
      }
    }

  }
}