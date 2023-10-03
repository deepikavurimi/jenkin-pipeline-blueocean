pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
ls
touch 1234.txt'''
      }
    }

    stage('test1') {
      parallel {
        stage('test1') {
          steps {
            echo 'hi all'
          }
        }

        stage('test2') {
          steps {
            sh 'echo "hello world"'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        sleep 30
      }
    }

  }
}