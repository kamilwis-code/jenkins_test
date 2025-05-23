pipeline {
    agent any

    stages {
        stage('Get Repo') {
            steps {
                git 'https://github.com/kamilwis-code/jenkins_test.git'
            }
        }

        stage('Launch python script') {
            steps {
                sh 'python3 main.py'
            }
        }
    }
}
