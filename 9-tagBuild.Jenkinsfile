pipeline {
    agent any

    stages {
        stage('Tag Build') {
            steps {
                script {
                    currentBuild.displayName = "#${currentBuild.number} - Meu Build"
                    currentBuild.description = "Build para implementar uma nova funcionalidade"
                    echo "Tags adicionadas à build"
                }
            }
        }
    }
}
