pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'building is happening'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'testing is happening'
          }
        }

        stage('test2') {
          steps {
            echo 'if test failed , try this'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploying is happening'
      }
    }

    

  }
}
