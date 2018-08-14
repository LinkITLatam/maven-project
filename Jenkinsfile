pipeline {
  agent any
  stages {
    stage('Say Hello') {
      parallel {
        stage('Say Hello') {
          steps {
            sh 'echo "Hello World"'
          }
        }
        stage('Say Goodbye') {
          steps {
            echo 'Goodbye'
          }
        }
      }
    }
  }
}