pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    echo "Executando build"
                    // Comandos de build
                }
            }
        }
    }

    post {
        success {
            slackSend channel: '#build-notifications', message: "Pipeline ${currentBuild.fullDisplayName} foi bem-sucedido."
        }
        failure {
            slackSend channel: '#build-notifications', message: "Pipeline ${currentBuild.fullDisplayName} falhou."
        }
    }
}
