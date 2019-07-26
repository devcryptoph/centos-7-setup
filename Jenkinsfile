pipeline {
  agent any
  stages {
    stage('Stage1') {
      steps {
        echo 'Hello'
      }
    }
    stage('Stage2') {
      steps {
        sh 'echo "Hello World"'
      }
    }
    stage('Stage3') {
      steps {
        input(message: 'Enter Name', id: 'name')
        sh '''echo "Building Custom VM"
echo "Done!"'''
      }
    }
  }
}