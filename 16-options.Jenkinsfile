pipeline {
    agent any

    options {
        timeout(time: 30, unit: 'MINUTES')
        buildDiscarder(logRotator(daysToKeepStr: '7', numToKeepStr: '10'))
        disableConcurrentBuilds()
    }

    stages {
        stage('Example') {
            steps {
                script {
                    echo "Exemplo de opções de pipeline"
                }
            }
        }
    }
}
