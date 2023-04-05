pipeline {
    agent any

    tools {
        // Install the Maven version configured as "M3" and add it to the path.
        maven "3.6.3"
    }

    stages {
        stage('Build') {
            steps {
                sh 'mvn clean package'
             
        }
    }
}
