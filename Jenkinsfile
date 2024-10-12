pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                echo 'Cloning the repository...'
                git 'https://github.com/Pythonshishir123/practice.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building the project...'
                // Insert build commands here, e.g., sh 'make build' or mvn build
            }
        }
        stage('Test') {
            steps {
                echo 'Running tests...'
                // Insert test commands here, e.g., sh 'make test' or mvn test
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
                // Insert deploy commands here, e.g., sh 'deploy script'
            }
        }
    }

    post {
        always {
            echo 'Cleaning up...'
            // Optional cleanup actions
        }
        success {
            echo 'Pipeline completed successfully.'
        }
        failure {
            echo 'Pipeline failed.'
        }
    }
}
