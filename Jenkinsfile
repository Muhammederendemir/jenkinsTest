node {

    try {
        sh 'might fail'
        echo 'Succeeded!'
    } catch (err) {
        echo "Failed: ${err}"
        echo "${BUILD.URL}"
        slackSend channel: '#jenkins',
                color: 'good',
                message: "Failed: ${err}"
    } finally {
        sh './tear-down.sh'
    }
    echo 'Printed whether above succeeded or failed.'

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

    }
    echo "RESULT: ${currentBuild.result}"
}