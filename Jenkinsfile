
pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Compiling Java application...'
                sh 'javac assignment.java'
            }
        }

        stage('Run Application') {
            steps {
                echo 'Running Java application...'
                sh 'java Assignment'
            }
        }
    }

    post {
        success {
            echo 'CI/CD Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed. Check the console output.'
        }
    }
}
