pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                slackSend: "Build Started"
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
    }
}