pipeline {
    agent any
    
    environment {
        GIT_CREDENTIALS = credentials('GITHUB_CREDENTIALS') // Utiliza la función credentials() para obtener las credenciales
    }
    
    stages {
        stage('Clonar Repositorio') {
            steps {
                script {
                    git credentials: GIT_CREDENTIALS, url: 'https://github.com/jake1331982/proyect-vla.git'
                }
            }
        }
        
        stage('Instalar Dependencias') {
            steps {
                script {
                    sh 'echo "Instalando dependencias..."'
                    // Aquí deberías agregar los comandos reales para instalar dependencias
                }
            }
        }
        
        stage('Ejecutar Pruebas') {
            steps {
                script {
                    sh 'echo "Ejecutando pruebas..."'
                    // Aquí deberías agregar los comandos reales para ejecutar las pruebas
                }
            }
        }
        
        stage('Construir Proyecto') {
            steps {
                script {
                    sh 'echo "Construyendo proyecto..."'
                    // Aquí deberías agregar los comandos reales para construir el proyecto
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
pipeline {
    agent any
    
    environment {
        GIT_CREDENTIALS = credentials('GITHUB_CREDENTIALS') // Utiliza la función credentials() para obtener las credenciales
    }
    
    stages {
        stage('Clonar Repositorio') {
            steps {
                script {
                    git credentials: GIT_CREDENTIALS, url: 'https://github.com/jake1331982/proyect-vla.git'
                }
            }
        }
        
        stage('Instalar Dependencias') {
            steps {
                script {
                    sh 'echo "Instalando dependencias..."'
                    // Aquí deberías agregar los comandos reales para instalar dependencias
                }
            }
        }
        
        stage('Ejecutar Pruebas') {
            steps {
                script {
                    sh 'echo "Ejecutando pruebas..."'
                    // Aquí deberías agregar los comandos reales para ejecutar las pruebas
                }
            }
        }
        
        stage('Construir Proyecto') {
            steps {
                script {
                    sh 'echo "Construyendo proyecto..."'
                    // Aquí deberías agregar los comandos reales para construir el proyecto
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
