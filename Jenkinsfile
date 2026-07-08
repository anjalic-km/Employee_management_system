pipeline {
    agent any

    stages {

        stage('Build Backend') {
            steps {
                dir('ems-backend') {
                   sh 'mvn clean package -DskipTests'
                }
            }
        }

        stage('Build Frontend') {
            steps {
                dir('ems-frontend') {
                    sh 'npm install'
                }
            }
        }
    }
}