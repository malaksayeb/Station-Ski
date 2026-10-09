pipeline {
    agent any
    stages {
        stage('Récupération du code') {
            steps {
                checkout scm
            }
        }
        stage('Affichage de la date') {
            steps {
                sh 'date'
            }
        }
    }
}
