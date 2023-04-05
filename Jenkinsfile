pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven 'maven'
        
        
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn -dmaven.test.failure.gnore=true install'   
            } 
            post {
                success {
                    junit 'target/surefire-reports/**/*.xml'
                }
            }
        }
    }
}
