pipeline {
    agent any
    
    tools {
       
        maven 'maven3'
    }

    stages {
        
        stage('Compile') {
            steps {
               sh "mvn compile"
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
        
        stage('Install') {
            steps {
                sh "mvn install"
            }
        }
    }
}
