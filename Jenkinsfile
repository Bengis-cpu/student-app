pipeline {
    agent any

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/Bengis-cpu/student-app.git'
            }
        }

        stage('Build') {
            steps {
                bat 'npm install'
            }
        }

        stage('Test') {
            steps {
                bat 'echo "No tests implemented"'
            }
        }

        stage('Docker Build') {
            steps {
                bat 'docker build -t student-app .'
            }
        }

        stage('Run Container') {
            steps {
                bat 'docker run -d -p 3000:3000 student-app'
            }
        }
    }
}