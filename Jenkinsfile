pipeline {
  agent any
  stages {
    stage('echo') {
      parallel {
        stage('echo') {
          steps {
            sh 'echo "shell Script echo ok"'
          }
        }
        stage('echo2') {
          steps {
            echo 'echo stegs 2'
          }
        }
      }
    }
    stage('maven') {
      steps {
        echo 'maven ok '
        echo 'are you ok'
      }
    }
    stage('done') {
      steps {
        sleep(time: 1, unit: 'SECONDS')
        echo 'maven test ok'
      }
    }
  }
}