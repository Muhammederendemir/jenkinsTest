node {
    try {
        // do something that doesn't fail
        echos
        echo "Im not going to fail"
        currentBuild.result = 'SUCCESS'
    } catch (Exception err) {
        currentBuild.result = 'FAILURE'
        echo err.toString()
    }
    echo "RESULT: ${currentBuild.result}"
}