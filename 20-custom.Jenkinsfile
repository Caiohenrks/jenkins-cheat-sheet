pipeline {
    agent {
        docker {
            image 'node:14-alpine'
            args '-v /path/to/local/dir:/path/to/container/dir'
        }
    }

    stages {
        stage('Build') {
            steps {
                script {
                    echo "Executando build dentro de um container Docker"
                    // Comandos de build
                }
            }
        }
    }
}
