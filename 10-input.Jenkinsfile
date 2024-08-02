pipeline {
    agent any

    stages {
        stage('Manual Approval') {
            steps {
                script {
                    input message: 'Aprovar para prosseguir?', ok: 'Sim, vamos em frente!'
                    echo "Aprovação manual recebida, continuando o pipeline"
                }
            }
        }
    }
}
