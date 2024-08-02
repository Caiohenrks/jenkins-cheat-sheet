pipeline {
    agent any

    stages {
        stage('Flaky Task') {
            steps {
                retry(3) {
                    script {
                        echo "Tentativa de executar uma tarefa que pode falhar"
                        if (new Random().nextBoolean()) {
                            error "Erro simulado!"
                        } else {
                            echo "Tarefa executada com sucesso"
                        }
                    }
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
                echo "Pipeline falhou após múltiplas tentativas."
            }
        }
    }
}
