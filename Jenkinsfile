

pipeline {
    agent any
    stages {

        stage('Example') {,
        steps{
            if (env.BRANCH_NAME == 'master') {
                slackSend baseUrl: 'https://hooks.slack.com/services/', channel: 'jenkins', color: 'good', iconEmoji: '', message: 'Brach master', teamDomain: 'javadevelopercorp58', tokenCredentialId: 'slack_Token_webhook', username: ''
            } else {
                echo 'I'
            }
            }
        }
    }
}