pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Démarrage du build...'
                bat 'node hello.js'
            }
        }
    }
}
