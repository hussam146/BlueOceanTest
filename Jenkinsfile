pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build Completed'
      }
    }

    stage('Test Flow') {
      parallel {
        stage('Test Flow') {
          steps {
            echo 'Test Flow entered'
          }
        }

        stage('Test1') {
          steps {
            echo 'Test1 completed'
          }
        }

        stage('Test2') {
          steps {
            echo 'Test2 completed'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        sh '''








echo $(date)


            








'''
      }
    }

    stage('Validate') {
      steps {
        input(message: 'Are You sure that you want to deploy', ok: 'Yes')
      }
    }

  }
}