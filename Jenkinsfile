

pipeline {
    agent any
    stages {
           stage('Slack Notification'){
                slackSend baseUrl: 'https://hooks.slack.com/services/', channel: 'jenkins', color: 'good', iconEmoji: '', message: 'Hello slack', teamDomain: 'javadevelopercorp58', tokenCredentialId: 'slack_Token_webhook', username: ''
        }
    }
}