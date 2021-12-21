pipeline {
  agent any
  options {
        ansiColor('xterm')
    }

  stages {
    stage('Ping Hosts') {
      steps {
        sh '''
          ansible all -i hosts -m ping
        '''
    }
    }
    stage('Install pacotes') {
      steps {
        sh '''
          ansible-playbook -i hosts playbook.yaml
        '''
    }
    }
  }
}