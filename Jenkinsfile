
pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o PES2UG20CS401-1 new.cpp'
                echo "Build Successful"
            }
        }
        stage('Test') {
            steps {
                sh 'PES2UG20CS401-1'
            }
        }
    }
    post {
        always {
            echo 'Pipeline completed'
        }
        failure {
            echo 'Pipeline failed'
        }
    }
}
