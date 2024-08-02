pipeline {
    agent any

    stages {
        stage('Parallel Execution') {
            parallel {
                stage('Stage 1') {
                    steps {
                        script {
                            echo "Executando estágio 1"
                            sleep(time: 1, unit: 'MINUTES')
                        }
                    }
                }
                stage('Stage 2') {
                    steps {
                        script {
                            echo "Executando estágio 2"
                            sleep(time: 1, unit: 'MINUTES')
                        }
                    }
                }
            }
        }
    }
}
