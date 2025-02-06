pipeline {
    agent any

    stages {
        stage('Pull Latest Code') {
            steps {
                git branch: 'main', url: 'https://github.com/NavinReigns/EvaMaria_V3.git'
            }
        }
        
        stage('Deploy to Server') {
            steps {
                script {
                    def deployPath = "D:\\Learnings\\pipeline\\EvaMaria_V3"
                    bat "xcopy /E /Y /I * ${deployPath}"
                }
            }
        }
    }
}
