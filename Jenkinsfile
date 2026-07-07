pipeline {
    agent any

    stages {

        stage('Build Backend') {
            steps {
                dir('ems-backend') {
                    sh 'mvn clean install'
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