pipeline {
    agent any

    stages {
        stage('Critical Section') {
            steps {
                lock('resource-name') {
                    script {
                        echo "Executando seção crítica com controle de concorrência"
                        // Comandos que devem ser executados com controle de concorrência
                    }
                }
            }
        }
    }
}
