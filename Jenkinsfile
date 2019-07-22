pipeline {
    agent any
    stages {
        stage('No-op') {
            steps {
                sh 'ls'
            }
        }
    }
    post {
        always {
            echo 'One way or another, I have finished'
            deleteDir() /* clean up our workspace */
        }
        success {
            echo 'I succeeeded!'
             slackSend baseUrl: 'https://hooks.slack.com/services/', channel: 'jenkins', color: 'blue', iconEmoji: '', message: 'I succeeeded!', teamDomain: 'javadevelopercorp58', tokenCredentialId: 'slack_Token_webhook', username: ''
        }
        unstable {
            echo 'I am unstable :/'
        }
        failure {
            echo 'I failed :('
        }
        changed {
            echo 'Things were different before...'
        }
    }
}