pipeline {
    agent any

    stages {
        stage('Simulated Failure') {
            steps {
                script {
                    echo "Simulando falha"
                    error "Erro simulado!"
                }
            }
        }
    }

    post {
        always {
            script {
                echo "Pipeline finalizada."
            }
        }
        failure {
            script {
                echo "Pipeline falhou. Executando ações de recuperação."
            }
        }
    }
}
