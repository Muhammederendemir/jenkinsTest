pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'echo "Hello World"'
                sh '''
                slackSend message: "Build Started"
                    echo "Multiline shell steps works too"
                    ls -lah
                '''
            }
        }
    }
}