pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                build 'PES2UG22CS043-1'
                sh 'g++ outdsfadsput.cpp -o output'
            }
        }
        
        stage('Test') {
            steps {
                sh './outfadsput'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploy'
            }
        }
    }

    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}
