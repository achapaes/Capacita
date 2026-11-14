pipeline {
    agent any
    stages {
        stage('Saludio e Información') {
            steps {
                echo '¡Hola Jenkins! Este es mi primer Job.'
                sh 'uname -a' // Muestra información del sistema operativo del contenedor
                sh 'java -version' // Verifica si Java está disponible
            }
        }
        stage('Simulando Compilación') {
            steps {
                echo 'Compilando código...'
                sh 'echo "Simulando compilación exitosa" > build.txt'
            }
        }
        stage('Pruebas') {
            steps {
                echo 'Ejecutando pruebas unitarias...'
                sh 'echo "Todas las pruebas pasaron"'
            }
        }
    }
    post {
        success {
            echo '¡El Pipeline se ejecutó exitosamente!'
        }
        failure {
            echo 'Algo salió mal en el proceso.'
        }
    }
}