pipeline {
    agent any

    options {
        buildDiscarder(logRotator(numToKeepStr: '10'))
        disableConcurrentBuilds()
    }

    stages {
        stage('Set Description') {
            steps {
                script {
                    currentBuild.description = "Este é um exemplo de descrição para a build"
                    echo "Descrição definida para a build"
                }
            }
        }
    }
}
