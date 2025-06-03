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
                    cd demo_app
                    docker build -t myapp .
                '''
            }
        }
    }
}
