pipeline {
    agent any

    stages {
        stage('Install Python') {
            steps {
                sh '''
                  sudo apt update
                  sudo apt install python3 -y
                '''
            }
        }

        stage('Run Python') {
            steps {
                sh 'python3 hello.py'
            }
        }
    }
}
