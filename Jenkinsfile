pipeline {
  agent any

  stages {
    stage('Hello') {
      steps {
        sh '''
          ansible -i hosts -m ping
        '''
      }
    }
  }
}