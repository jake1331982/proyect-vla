pipeline {
    agent any
        
    
    environment {
        GIT_CREDENTIALS = 'GITHUB_CREDENTIALS'  // Reemplaza con el ID de tus credenciales
    }
    stages {
        stage('Clonar Repositorio') {
            steps {
                script {
                    git credentialsId: env.GIT_CREDENTIALS, url: 'https://github.com/jake1331982/proyect-vla.git'
                }
            }
        }
        stage('Instalar Dependencias') {
            steps {
                script {
                    "echo 'hola'"
                }
            }
        }
        stage('Ejecutar Pruebas') {
            steps {
                script {
                    sh "echo 'hola'"
                }
            }
        }
        stage('Construir Proyecto') {
            steps {
                script {
                    sh "echoJenkinsfile 'hola'"
                }
            }
        }
    }
    post {Jenkinsfile
        success {
            echo 'Pipeline ejecutado con éxito.'
        }
        failure {
            echo 'El pipeline ha fallado.'
        }
    }
}
