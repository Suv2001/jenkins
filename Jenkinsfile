pipeline {
    agent any

    stages {
        stage('Install Python') {
            steps {
                sh '''
                  echo "your-password" | sudo -S apt update
                  echo "your-password" | sudo -S apt install python3 -y
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
