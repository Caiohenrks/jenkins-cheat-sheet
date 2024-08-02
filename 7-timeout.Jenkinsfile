pipeline {
    agent any

    stages {
        stage('Long Running Task') {
            steps {
                timeout(time: 5, unit: 'MINUTES') {
                    script {
                        echo "Executando tarefa de longa duração"
                        sleep(time: 10, unit: 'MINUTES')
                    }
                }
            }
        }
    }

    post {
        always {
            script {
                echo "Pipeline finalizada."
            }
        }
        aborted {
            script {
                echo "Pipeline foi abortada devido ao timeout."
            }
        }
    }
}
