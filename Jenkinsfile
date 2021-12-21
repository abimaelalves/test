pipeline {
  agent any

  stages {
    stage('Hello') {
      steps {
        sh '''
          ansible all -i hosts -m ping
        '''
      }
    }
  }
}