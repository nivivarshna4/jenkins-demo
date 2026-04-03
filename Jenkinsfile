pipeline {
    agent any

    environment {
        APP_NAME = "MyApp"
    }

    stages {

        stage('Install') {
            steps {
                echo 'Installing dependencies'
            }
        }

        stage('Build') {
            steps {
                echo "Building ${APP_NAME}"
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests'
            }
        }

        stage('Quality Check') {
            steps {
                echo 'Checking code quality (SonarQube simulation)'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying application'
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished'
        }
        success {
            echo 'Build Success'
        }
        failure {
            echo 'Build Failed'
        }
    }
}
