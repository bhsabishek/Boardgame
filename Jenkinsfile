pipeline {
    agent { label 'slave1'}
     
    tools {
        maven 'maven3.9.10'
        jdk 'jdk17'
    }

    stages {
        
        stage('Compile') {
            steps {
             sh 'mvn compile'
            }
        }
        
        stage('Test') {
            steps {
              sh 'mvn test' 
            }
        }
        
        stage('Build') {
            steps {
              sh "mvn package"
            }
        }
    }
}
