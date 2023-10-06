pipeline {
    agent any

    environment {
        AWS_DEFAULT_REGION = 'ap-south-1'
        AWS_ACCESS_KEY_ID = credentials('AKIARGWR6CGS3SJQEKM4')
        AWS_SECRET_ACCESS_KEY = credentials('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')
    }

    stages {
        stage('Checkout') {
            steps {
                script {
                    // Checkout code from AWS CodeCommit
                    def codeCommitUrl = 'https://git-codecommit.ap-south-1.amazonaws.com/v1/repos/Snapcoins'
                    git branch: 'main', credentialsId: '65b859fa-8c76-49a5-b70c-53b42326b02c', url: 'https://git-codecommit.ap-south-1.amazonaws.com/v1/repos/Snapcoin'
                }
            }
        }

        
    }

    
}
