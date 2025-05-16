pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo "Build and run the NodeJS web application with npm"
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo "Running unit and integration tests with Mocha & Chai"
            }
        }

        stage('Code Analysis') {
            steps {
                echo "Check the quality of the code with ESLint"
            }
        }

        stage('Security Scan') {
            steps {
                echo "Perform code security scanning with npm audit"
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo "Deploy Staging to Heroku [STAG]"
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo "Running integration tests on staging with Mocha & Chai"
            }
        }

        stage('Deploy to Production') {
            steps {
                echo "Deploy Production to Heroku [PROD]"
            }
        }
    }
}
