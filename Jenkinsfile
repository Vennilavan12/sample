pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven 'maven 3.6.3'
        jdk 'jdk11'
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
            }   
        }
    }
}
