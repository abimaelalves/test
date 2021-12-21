pipeline {
    agent any
    }

    stages {
        stage('Test Ping ansible') {
            steps {
                sh "ansible -i hosts -m ping"
            }
        }
    }
}