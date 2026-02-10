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
                sh 'mvn clean compile'
            }
        }

        stage('Run') {
            steps {
                sh 'mvn exec:java'
            }
        }
    }
}
