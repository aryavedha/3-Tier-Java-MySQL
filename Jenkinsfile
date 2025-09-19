pipeline {
    agent any
    
    tools {
        maven 'mvn'
        jdk 'java17'
    }

    stages {
         stage('compile') {
            steps {
                sh 'mvn compile'
            }
        }

        stage('test') {
            steps {
                sh 'mvn test'
            }
        }
        stage('package') {
            steps {
                sh 'mvn package'
            }
        }
        stage('success') {
            steps {
                echo 'success'
            }
        }
    }
}
