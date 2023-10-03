pipeline {
    agent any

    stages {
        stage('Clonar Repositorio') {
            steps {
                // Clonar el repositorio de GitHub
                git 'https://github.com/tu-usuario/tu-repositorio.git'
            }
        }

        stage('Construir y Empaquetar') {
            steps {
                // Ejecutar comandos para construir tu aplicación
                sh 'docker build -t mi-app .'
            }
        }

        stage('Desplegar en Producción') {
            steps {
                // Desplegar la aplicación utilizando Docker Compose
                sh 'docker-compose up -d'
            }
        }
    }
}
