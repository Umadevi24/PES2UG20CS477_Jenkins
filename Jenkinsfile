pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES2UG20CS477-1 try.cpp'
                echoo "Build Successful"
            }
        }
        stage('Test') {
            steps {
                sh './PES2UG20CS477-1'
            }
        }
    }
    post {
        always {
            echoo 'Pipeline completed'
        }
        failure {
            echoo 'Pipeline failed'
        }
    }
}
