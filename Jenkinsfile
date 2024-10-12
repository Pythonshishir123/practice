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

