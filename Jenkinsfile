pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Build') {
            steps {
                script {
                    sh './gradlew build'
                }
            }
        }

        // Ajoutez d'autres étapes selon vos besoins (tests, déploiement, etc.).
    }

    post {
        always {
            // Ajoutez des étapes qui doivent être exécutées même en cas d'échec.
        }
    }
}
