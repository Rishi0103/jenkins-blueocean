pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Hello this is Rishikesh'
        echo 'welcome'
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            sh '''ls
pwd
date
cal 2023'''
          }
        }

        stage('test2') {
          steps {
            echo 'this is test 2'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
        sleep 10
      }
    }

  }
  environment {
    name = 'Rishi'
  }
}