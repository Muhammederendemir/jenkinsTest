node {
    try {
        // do something that doesn't fail
        echos
        echo "Im not going to fail"
        currentBuild.result = 'SUCCESS'
    } catch (Exception err) {
        currentBuild.result = 'FAILURE'
         err.getMessage()
    }
    echo "RESULT: ${currentBuild.result}"
}