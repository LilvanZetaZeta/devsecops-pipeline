pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Iniciando fase de Build...'
                echo 'Compilando el código fuente del Hello World'
                // Aquí irían comandos reales como 'npm install' o 'mvn clean compile'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Iniciando fase de Test...'
                echo 'Ejecutando pruebas unitarias y de seguridad básica'
                // Aquí irían comandos como 'npm test' o análisis de SonarQube
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Iniciando fase de Deploy...'
                echo 'Desplegando la aplicación en el entorno de prueba'
                // Como ya integramos Docker en el paso anterior, podemos simular el despliegue
                sh 'docker run --rm hello-world'
            }
        }
    }
}
