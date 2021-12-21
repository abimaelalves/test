pipeline {
    agent any
    
    stages {
        stage('Deploying Ansible') {
            steps {
                sh "sudo ansible-playbook /home/ubuntu/ansible-lives/playbook-ec2.yml --extra-vars='nameinvault=$params.NAMEINST'"
            }
        }
    }
}