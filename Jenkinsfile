pipeline {
  agent any
  stages {
    stage('Test') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'hello'
          }
        }

        stage('builld_parallel') {
          steps {
            echo 'jjjj'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'mmmm'
      }
    }

    stage('hhh') {
      parallel {
        stage('hhh') {
          steps {
            echo 'fghh'
            sleep 10
          }
        }

        stage('ggg') {
          steps {
            sh 'pwd'
          }
        }

      }
    }

  }
}