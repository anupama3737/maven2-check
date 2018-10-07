node {
    // Clean workspace before doing anything
    deleteDir()

    try {
        stage ('Job1') {
            echo "I'm job1"
        }
        stage ('Job2') {
            echo "I'm job2"
        }
       
        stage ('Job3') {
            echo "I'm job3"
            sh "echo 'hello.sh'"
        }
    } catch (err) {
        currentBuild.result = 'FAILED'
        throw err
    }
}
