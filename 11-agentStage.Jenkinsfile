pipeline {
    agent none

    stages {
        stage('Build') {
            agent { label 'build-agent' }
            steps {
                script {
                    echo "Executando build no agente específico 'build-agent'"
                    // Comandos de build
                }
            }
        }
        stage('Test') {
            agent { label 'test-agent' }
            steps {
                script {
                    echo "Executando testes no agente específico 'test-agent'"
                    // Comandos de teste
                }
            }
        }
    }
}
