

pipeline {
    agent any
    stages {
           stage('Slack Notification'){
           steps{
                slackSend baseUrl: 'https://hooks.slack.com/services/', channel: 'jenkins', color: 'good', iconEmoji: '', message: 'Hello slack', teamDomain: 'javadevelopercorp58', tokenCredentialId: 'slack_Token_webhook', username: ''
                  slackSend baseUrl: 'https://hooks.slack.com/services/', channel: 'general', color: 'red', iconEmoji: '', message: 'slack meşaj işlemi çalışıyor', teamDomain: 'javadevelopercorp58', tokenCredentialId: 'slack_Token_webhook', username: ''
        }
        }
    }
}