pipeline {
    agent any


    stages {
        stage("Build") {
            steps {
                sh 'chmod 777 mvnw'
                sh "./mvnw -version"
                sh "./mvnw clean install"
            }
        }
    }

}