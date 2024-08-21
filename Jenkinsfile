pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://shivamcanqualify@bitbucket.org/canqualify/multi-branch.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the application...'
            }
        }
    }

    post {
        success {
            echo 'Build succeeded!'
        }
        failure {
            echo 'Build failed.'
        }
    }
}
