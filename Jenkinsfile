pipeline{
    agent any

    stages{

         stage('Build') {
                    steps {
                        sh 'make' (1)
                        archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true (2)
                    }
                }
    }
}