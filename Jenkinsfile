pipeline {
  agent any
  stages {
    stage('Bulid') {
      steps {
        echo 'Bulid completed'
      }
    }

    stage('Test Stages') {
      parallel {
        stage('Test 2') {
          steps {
            echo 'running test 2'
          }
        }

        stage('Test 1') {
          steps {
            echo 'running test1'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployment completed'
      }
    }

  }
}