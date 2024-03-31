pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                // Build Docker image
                script {
                    docker.build("my-python-app:latest")
                }
            }
        }
        stage('Deploy') {
            steps {
                // Deploy Docker image
                script {
                    docker.image("my-python-app:latest").run()
                }
            }
        }
    }
}
