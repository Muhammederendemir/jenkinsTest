

pipeline {
    agent any
    stages {
           stage('Slack Notification'){
                slackSend baseUrl: 'https://hooks.slack.com/services/', channel: 'jenkins', color: 'good', iconEmoji: '', message: 'Hello slack', teamDomain: 'Java Developer', tokenCredentialId: 'slack_Token_webhook', username: ''
        }
    }
}