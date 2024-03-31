pipeline {
    agent any
    stages {
        stage('Test') {
            steps {
                script {
                    echo "Testing...")
                }
            }
        }
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
