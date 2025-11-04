pipeline {
    agent any
    
    tools {
        maven 'Maven-3.9.11'
        jdk 'jdk17'
    }

    stages {
        
        stage('Compile') {
            steps {
            sh  "mvn compile"
            }
        }
        
        stage('Test') {
            steps {
                sh "mvn test"
            }
        }
        
        stage('Package') {
            steps {
                sh "mvn package"
            }
        }
    }
}
