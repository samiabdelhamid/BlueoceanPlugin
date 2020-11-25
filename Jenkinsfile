pipeline {
  agent any
  stages {
    stage('Build Stage') {
      steps {
        echo 'Build Copleted'
      }
    }

    stage('Test Stage') {
      parallel {
        stage('Test Phase 1') {
          steps {
            echo 'Testing Start'
          }
        }

        stage('Testing Phase 2') {
          steps {
            echo 'Testing Complete'
          }
        }

      }
    }

    stage('Deploy Stage') {
      steps {
        echo 'Deploy Complete'
        input(message: 'Are you sure want deploy', ok: 'i am sure')
      }
    }

    stage('Commit Stage') {
      steps {
        echo 'Commit'
      }
    }

  }
}