pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
                echo 'Source code checked out successfully'
            }
        }

        stage('Validate Dockerfile') {
            steps {
                sh 'test -f Dockerfile'
                echo 'Dockerfile found successfully'
            }
        }
    }
}
