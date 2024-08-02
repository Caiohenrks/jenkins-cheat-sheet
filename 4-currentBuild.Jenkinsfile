pipeline {
    agent any

    stages {
        stage('Current Build Info') {
            steps {
                script {
                    echo "Número da Build: ${currentBuild.number}"
                    echo "Status da Build: ${currentBuild.currentResult}"
                    currentBuild.description = "Build executada com sucesso"
                    echo "Descrição da Build: ${currentBuild.description}"
                }
            }
        }
    }
}
