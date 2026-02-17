pipeline {
    agent any

   
    tools {
    maven 'Maven'
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/joshishrau/Github_Jenkins.git'
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
