pipeline {
  agent any

  stages {
    stage('Ping Hosts') {
      steps {
        sh '''
          ansible all -i hosts -m ping
        '''
      }
    }
  }
}