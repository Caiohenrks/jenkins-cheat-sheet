pipeline {
    agent any

    environment {
        // Variáveis de ambiente
        MY_VAR = 'Valor da minha variável'
    }

    stages {
        stage('Use Variable') {
            steps {
                script {
                    echo "Valor da variável MY_VAR: ${env.MY_VAR}"
                }
            }
        }
    }
}
