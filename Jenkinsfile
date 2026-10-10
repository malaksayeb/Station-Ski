pipeline {
    agent any

    stages {
        stage('Récupération du Jenkinsfile et du code') {
            steps {
                checkout([
                    $class: 'GitSCM',
                    branches: [[name: '*/main']], // Remplace 'main' par 'master' si ta branche principale s'appelle master
                    userRemoteConfigs: [[url: 'https://github.com/malaksayeb/Station-Ski-Pipeline.git']]
                ])
            }
        }

        stage('Affichage de la date') {
            steps {
                sh 'date'
            }
        }
    }
}
