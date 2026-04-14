pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                git 'https://github.com/harSHITags/Retail-RAG-Chatbot'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip install -r requirements.txt'
            }
        }

        stage('Build Docker Image') {
            steps {
                sh 'docker build -t retail-ai-app .'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deployment step will be added (Kubernetes)'
            }
        }
    }
}