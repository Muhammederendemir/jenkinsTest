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
        echo"gıthubbbbb"
        echo "BUILD_NUMBER" :: $BUILD_NUMBER
        echo "BUILD_ID" :: $BUILD_ID
        echo "BUILD_DISPLAY_NAME" :: $BUILD_DISPLAY_NAME
        echo "JOB_NAME" :: $JOB_NAME
        echo "JOB_BASE_NAME" :: $JOB_BASE_NAME
        echo "BUILD_TAG" :: $BUILD_TAG
        echo "EXECUTOR_NUMBER" :: $EXECUTOR_NUMBER
        echo "NODE_NAME" :: $NODE_NAME
        echo "NODE_LABELS" :: $NODE_LABELS
        echo "WORKSPACE" :: $WORKSPACE
        echo "JENKINS_HOME" :: $JENKINS_HOME
        echo "JENKINS_URL" :: $JENKINS_URL
        echo "BUILD_URL" ::$BUILD_URL
        echo "JOB_URL" :: $JOB_URL

    }
    echo "RESULT: ${currentBuild.result}"
}