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
        echo "${evn.GIT_COMMIT}"
        echo "${evn.GIT_PREVIOUS_COMMIT}"
        echo "${evn.GIT_PREVIOUS_SUCCESSFUL_COMMIT}"
        echo "${evn.GIT_BRANCH}"
        echo "${evn.GIT_LOCAL_BRANCH}"
        echo "${evn.GIT_COMMITTER_NAME}"
        echo "${evn.GIT_AUTHOR_NAME}"

    }
    echo "RESULT: ${currentBuild.result}"
}