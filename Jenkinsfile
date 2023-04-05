pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven 'maven'
        jdk 'java-11-openjdk-amd64'
        
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }   
        }
    }
}
