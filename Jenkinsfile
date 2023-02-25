pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed'
      }
    }

    stage('Test stages') {
      parallel {
        stage('Test stages') {
          steps {
            echo 'runnig'
          }
        }

        stage('Test1') {
          steps {
            echo 'runnig test1'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deployment'
      }
    }

  }
}