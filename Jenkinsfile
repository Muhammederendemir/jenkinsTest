node {
    try {
        // do something that doesn't fail
        echo's'
        echo "Im not going to fail"
        currentBuild.result = 'SUCCESS'
    } catch (Exception err) {
        currentBuild.result = 'FAILURE'
        echo "{evn.err}"
    }
    echo "RESULT: ${currentBuild.result}"
}