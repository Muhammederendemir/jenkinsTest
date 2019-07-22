node {

    try {
        // do something that doesn't fail
        echos
        echo "Im not going to fail"
        currentBuild.result = 'SUCCESS'
    } catch (Exception err) {
        currentBuild.result = 'SUCCESS'
         echo "hata"
            slackSend channel: '#jenkins',
                            color: 'good',
                            message: err.getMessage()
        echo err.getMessage()
        echo "gıthubbbbb"
        echo "BUILD_NUMBER ${env.BUILD_ID}"
        echo "BUILD_NUMBER ${env.BUILD_DISPLAY_NAME}"
        echo "BUILD_NUMBER ${env.$JOB_BASE_NAME}"
        echo "BUILD_NUMBER ${env.BUILD_TAG}"
        echo "BUILD_NUMBER ${env.EXECUTOR_NUMBER}"
        echo "BUILD_NUMBER ${env.NODE_NAME}"
        echo "BUILD_NUMBER ${env.NODE_LABELS}"
        echo "BUILD_NUMBER ${env.WORKSPACE}"
        echo "BUILD_NUMBER ${env.JENKINS_HOME}"
        echo "BUILD_NUMBER ${env.JENKINS_URL}"
        echo "BUILD_NUMBER ${env.JOB_URL}"

    }
    echo "RESULT: ${currentBuild.result}"
}