pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/your-username/event-registration-form.git'
            }
        }
        stage('Build') {
            steps {
                bat 'echo Building project in Windows!'
            }
        }
        stage('Test') {
            steps {
                bat 'echo Running basic tests'
            }
        }
        stage('Deploy') {
            steps {
                bat 'copy index.html C:\\path\\to\\deploy\\folder'
            }
        }
    }
    post {
        success {
            echo 'Pipeline completed successfully!'
        }
        failure {
            echo 'Pipeline failed!'
        }
    }
}
