pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/joshishrau/Github_Jenkins.git'
            }
        }

        stage('Build') {
            steps {
                bat 'mvn clean compile'
            }
        }

        stage('Run') {
            steps {
                bat 'mvn exec:java'
            }
        }
    }
}
