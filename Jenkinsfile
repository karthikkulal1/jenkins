pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo "Pulling code from GitHub..."
                git branch: 'main', url: 'https://github.com/<your-username>/<your-repo>.git'
            }
        }

        stage('Build') {
            steps {
                echo "Running Build Stage..."
                sh 'echo Building project...'   // Replace with your build command
            }
        }

        stage('Test') {
            steps {
                echo "Running Test Stage..."
                sh 'echo Running tests...'     // Replace with actual test script
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploy Stage Started..."
                sh 'echo Deploying application...'   // Replace with your deploy command
            }
        }
    }

    post {
        success {
            echo "Pipeline completed successfully!"
        }
        failure {
            echo "Pipeline failed!"
        }
    }
}
