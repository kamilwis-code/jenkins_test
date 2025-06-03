pipeline {
    agent any

    stages {

        stage('Launch python script') {
            steps {
                sh 'python3 main.py'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh '''
                    docker build -t myapp ./demo_app
                '''
            }
        }
    }
}
