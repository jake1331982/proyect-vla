
pipeline {
    agent any
    
    
    stages {
        stage("Clonar Repositorio") {
            steps {
                script {
                    git credentialsId: 'GITHUB_CREDENTIAL', url: 'https://github.com/jake1331982/proyecto-vla.git'
                }
            }
        }
        stage("Ejecutar Comando") {
            steps {
                script {
                    sh "echo 'hola'"
                }
            }
        }
    }
    post {
        success {
            echo 'Pipeline ejecutado con éxito.'
        }
        failure {
            echo 'El pipeline ha fallado.'
        }
    }
}
