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
      success {
          slackSend channel: '#jenkins',
                    color: 'good',
                    message: "The pipeline ${currentBuild.fullDisplayName} completed successfully."
      }
  }
}