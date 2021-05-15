pipeline {
    agent any


    stages {
        stage("Build") {
            steps {
                sh 'chmod 777 mvnw'
                sh "./mvnw -version"
                sh "./mvnw clean install"
                sh "docker build --build-arg JAR_FILE=build/libs/\\*.jar -t springio/gs-spring-boot-docker ."
                sh "docker build -t springio/gs-spring-boot-docker ."

            }
        }
    }

}