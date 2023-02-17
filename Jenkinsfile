pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ try.cpp'
                echo "Build Successful"
            }
        }
        stage('Test') {
            steps {
                sh './PES2UG20CS477-1'
            }
        }
    }
     post{
        alw{
            echo 'Pipeline completed'
        }
        failu {
            echo 'Pipeline failed'
        }
    }
}

