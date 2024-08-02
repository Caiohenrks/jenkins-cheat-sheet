pipeline {
    agent any

    stages {
        stage('Load Config') {
            steps {
                script {
                    def config = readYaml file: 'config.yaml'
                    echo "Configuração carregada: ${config}"
                    // Use a configuração carregada conforme necessário
                }
            }
        }
    }
}
