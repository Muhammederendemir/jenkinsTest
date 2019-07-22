node {
    try {
        // do something that doesn't fail
        echos
        echo "Im not going to fail"
        currentBuild.result = 'SUCCESS'
    } catch (Exception err) {
        currentBuild.result = 'FAILURE'
         echo "hata"
            slackSend channel: '#jenkins',
                            color: 'good',
                            message: err.getMessage()
        echo    err.getMessage()

    }
    echo "RESULT: ${currentBuild.result}"
}