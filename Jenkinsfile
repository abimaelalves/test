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
    stage('Ping Hosts2') {
      steps {
        sh '''
          ansible all -i hosts -m ping
        '''
    }
    }
  }
}