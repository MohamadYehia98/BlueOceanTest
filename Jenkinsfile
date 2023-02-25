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
        input(message: 'Are you sure?', ok: 'Yes , i am sure')
        echo 'Deployment'
      }
    }

    stage('Notify') {
      steps {
        echo 'new build comp,'
      }
    }

  }
}