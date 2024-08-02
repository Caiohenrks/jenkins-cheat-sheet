pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                script {
                    echo "Executando build"
                    // Simulação de criação de artefato
                    writeFile file: 'artifact.txt', text: 'Este é um artefato de exemplo'
                }
            }
        }
        stage('Archive Artifacts') {
            steps {
                archiveArtifacts artifacts: 'artifact.txt', fingerprint: true
                echo "Artefato arquivado"
            }
        }
    }
}
