pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'main',
                url: 'https://github.com/anjalic-km/Employee_management_system.git'
            }
        }

        stage('Build Backend') {
            steps {
                dir('ems-backend') {
                    bat 'mvn clean install'
                }
            }
        }

        stage('Build Frontend') {
            steps {
                dir('ems-frontend') {
                    bat 'npm install'
                }
            }
        }
    }
}