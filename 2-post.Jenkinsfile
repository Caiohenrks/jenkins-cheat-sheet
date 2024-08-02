pipeline {
    agent any

    stages {
        stage('Success Example') {
            steps {
                script {
                    echo "Este estágio sempre será bem-sucedido"
                }
            }
        }
        stage('Failure Example') {
            steps {
                script {
                    echo "Simulando falha"
                    error "Erro simulado!"
                }
            }
        }
    }

    post {
        success {
            script {
                echo "Pipeline executado com sucesso!"
            }
        }
        failure {
            script {
                echo "Pipeline falhou. Executando ações de recuperação."
            }
        }
        always {
            script {
                echo "Ações que sempre são executadas"
            }
        }
    }
}
