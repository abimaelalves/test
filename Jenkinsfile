pipeline {
    agent any
    
    stages {
        stage('Deploying Ansible') {
            steps {
                sh "ansible -i host -m ping'"
            }
        }
    }
}