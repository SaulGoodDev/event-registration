pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/SaulGoodDev/event-registration.git'
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
                bat 'copy jukhn.html D:\Courses'
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
