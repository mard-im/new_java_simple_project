pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                git(
                   url: 'https://github.com/mard-im/new_java_simple_project.git',
                   credentialsId: '4c8afdd5-cc47-42d7-9a74-df219f6c82a9',
                   branch: "main"
                )
                sh 'chmod 777 mvnw'
                sh './mvnw clean compile'
            }
        }
    }
}
