pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                sendNotifications 'STARTED'
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
    }
}