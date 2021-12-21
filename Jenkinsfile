pipeline {
  agent any
  options {
        ansiColor('xterm')
    }

  stages {
    stage('Ping Hosts') {
      steps {
        sh '''
          export ANSIBLE_FORCE_COLOR=true
          ansible all -i hosts -m ping
        '''
    }
    }
    stage('Install pacotes') {
      steps {
        sh '''
          export ANSIBLE_FORCE_COLOR=true
          ansible-playbook -i hosts playbook.yaml -vv
        '''
    }
    }
  }
}