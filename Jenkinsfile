pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Démarrage du build...'
            }
        }
        stage('Test'){
            steps {
                script {
                    def fileExists = fileExists('index.html')
                    if (fileExists) {
                        echo 'Le fichier index.html existe.'
                    } else {
                        error ('Le fichier index.html n\'existe pas !')
                    }
                }
            }
        }
    }
}
