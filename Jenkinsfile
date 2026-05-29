pipeline {
    agent any
    stages {

        stage('Clone Code') {
            steps {
                git branch: 'main', url: 'https://github.com/sai-123-123/Devops-project'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build Next.js App') {
            steps {
                sh 'npm run build'
            }
        }

    }
}
