pipeline {
    agent any  // Use any available agent

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/mingyuzhao/simple-java-maven-app.git'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the application...'
            }
        }
    }
}
