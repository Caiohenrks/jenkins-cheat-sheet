pipeline {
    agent any

    environment {
        DEPLOY_ENV = 'production'
    }

    stages {
        stage('Deploy') {
            when {
                environment name: 'DEPLOY_ENV', value: 'production'
            }
            steps {
                script {
                    echo "Executando deploy em ambiente de produção"
                }
            }
        }
        stage('Skip Deploy') {
            when {
                environment name: 'DEPLOY_ENV', value: 'staging'
            }
            steps {
                script {
                    echo "Deploy em ambiente de staging, nada a fazer"
                }
            }
        }
    }
}
