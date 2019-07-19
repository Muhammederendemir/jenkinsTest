pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                sendNotifications 'STARTED1'
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
    }
}