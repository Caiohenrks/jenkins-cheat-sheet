pipeline {
    agent any

    stages {
        stage('Use Credentials') {
            steps {
                withCredentials([usernamePassword(credentialsId: 'my-credentials-id', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')]) {
                    script {
                        echo "Usando credenciais: ${USERNAME}"
                        // Comandos que utilizam as credenciais
                    }
                }
            }
        }
    }
}
