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

    stages {
    stage('Ping Hosts') {
      steps {
        sh '''
          ansible-playbook -i hosts playbook.yaml
        '''
      }
    }
  }
}