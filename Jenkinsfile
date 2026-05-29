pipeline {
    agent any

    environment {
        NEXT_PUBLIC_SUPABASE_URL = "YOUR_SUPABASE_URL"
        NEXT_PUBLIC_SUPABASE_ANON_KEY = "YOUR_SUPABASE_ANON_KEY"
    }

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
