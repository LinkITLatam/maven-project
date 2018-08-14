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
    stage('Mix') {
      steps {
        input(message: 'Are you ok?', id: 'ok', ok: 'Okeyy', submitter: 'mferrari', submitterParameter: 'mferrari')
        isUnix()
        pwd(tmp: true)
      }
    }
  }
}