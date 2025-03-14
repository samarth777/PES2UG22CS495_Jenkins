pipeline {
    agent any
    
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES2UG22CS495-1 ./main/hello.cpp'
                echo 'Build stage successful'
            }
        }
        stage('Test') {
            steps {
                sh './PES2UG22CS495-1'
                echo 'Test stage successful'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deployment successful'
            }
        }
    }
    
    post {
        failure {
            echo 'Pipeline failed'
        }
    }
}