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
        echo "BUILD_ID ${env.BUILD_ID}"
        echo "BUILD_DISPLAY_NAME ${env.BUILD_DISPLAY_NAME}"
        echo "JOB_BASE_NAME ${env.$JOB_BASE_NAME}"
        echo "BUILD_TAG ${env.BUILD_TAG}"
        echo "EXECUTOR_NUMBER ${env.EXECUTOR_NUMBER}"
        echo "NODE_NAME ${env.NODE_NAME}"
        echo "NODE_LABELS ${env.NODE_LABELS}"
        echo "WORKSPACE ${env.WORKSPACE}"
        echo "JENKINS_HOME ${env.JENKINS_HOME}"
        echo "JENKINS_URL ${env.JENKINS_URL}"
        echo "GIT_COMMIT ${env.GIT_COMMIT}"
        echo ".GIT_PREVIOUS_COMMIT ${env.GIT_PREVIOUS_COMMIT}"
        echo "GIT_PREVIOUS_SUCCESSFUL_COMMIT ${env.GIT_PREVIOUS_SUCCESSFUL_COMMIT}"
        echo ".GIT_BRANCH ${env.GIT_BRANCH}"
        echo "GIT_LOCAL_BRANCH ${env.GIT_LOCAL_BRANCH}"
        echo "GIT_URL ${env.GIT_URL}"
        echo "GIT_COMMITTER_NAME ${env.GIT_COMMITTER_NAME}"
        echo "GIT_AUTHOR_NAME ${env.GIT_AUTHOR_NAME}"


        mail to: 'mhmmderen2@gmail.com',
                subject: "Example Build: ${env.JOB_NAME} - Succe0ess",
                body: "Job Failed - \"${env.JOB_NAME}\"\n\n " +
                        "Build Number: ${env.BUILD_NUMBER}\n\n " +
                        "Build Url :\n ${env.BUILD_URL}\n\n\n\n"
    }
}
