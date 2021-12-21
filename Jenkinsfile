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

    stage('Ping Hosts') {
      steps {
        sh '''
          ansible-playbook -i hosts playbook.yaml
        '''
      }
    }
  
}