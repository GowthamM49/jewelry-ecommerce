pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/GowthamM49/jewelry-ecommerce.git'
            }
        }

        stage('Install Backend') {
            steps {
                dir('backend') {
                    bat 'npm install'
                }
            }
        }

        stage('Install Frontend') {
            steps {
                dir('frontend') {
                    bat 'npm install'
                }
            }
        }

        stage('Build') {
            steps {
                echo "Build completed"
            }
        }

        stage('Deploy') {
            steps {
                echo "Deployment step"
            }
        }
    }
}
