pipeline {
    agent any

    tools {
        maven 'Maven-3.9.6'
    }

    stages {
        stage('Compile') {
            steps {
                sh 'mvn -version'
                sh 'mvn compile'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn package'
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }
    }
}
