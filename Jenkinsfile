pipeline {
    agent any

    environment {
        DIRECTORY_PATH = "/path/to/source/code"
        TESTING_ENVIRONMENT = "Staging"
        PRODUCTION_ENVIRONMENT = "Hai Son Tran"
    }

    stages {
        stage('Build') {
            steps {
                echo "Fetch the source code from the directory path specified by the environment variable: ${env.DIRECTORY_PATH}"
                echo "Compile the code and generate any necessary artefacts"
            }
        }

        stage('Test') {
            steps {
                echo "Unit tests"
                echo "Integration tests"
            }
        }

        stage('Code Quality Check') {
            steps {
                echo "Check the quality of the code"
            }
        }

        stage('Deploy') {
            steps {
                echo "Deploy the application to a testing environment specified by the environment variable: ${env.TESTING_ENVIRONMENT}"
            }
        }

        stage('Approval') {
            steps {
                sleep time: 10, unit: 'SECONDS'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo "Deploying code to production environment: ${env.PRODUCTION_ENVIRONMENT}"
            }
        }
    }
}
