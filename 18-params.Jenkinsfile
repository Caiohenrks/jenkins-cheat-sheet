pipeline {
    agent any

    parameters {
        string(name: 'BRANCH', defaultValue: 'master', description: 'Branch a ser construído')
        booleanParam(name: 'RUN_TESTS', defaultValue: true, description: 'Executar testes?')
    }

    stages {
        stage('Checkout') {
            steps {
                script {
                    echo "Branch selecionado: ${params.BRANCH}"
                    // Comandos de checkout
                }
            }
        }
        stage('Test') {
            when {
                expression { return params.RUN_TESTS }
            }
            steps {
                script {
                    echo "Executando testes"
                    // Comandos de teste
                }
            }
        }
    }
}
