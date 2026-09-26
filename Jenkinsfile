pipeline {
    agent any
    tools {
        jdk 'jdk21'
        maven 'maven3.9'
    }

    stages {
       
        stage('Compilation') {
            steps {
                sh 'mvn compile'
            }
        }
        stage('Tests') {
            steps {
                sh 'mvn test'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
