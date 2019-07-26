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
        input(message: 'Proceed? ', id: 'ans', ok: 'Build!')
        sh '''echo "Building Custom VM"
echo "Done!"'''
      }
    }
  }
}