pipeline {
    agent any
    environment {
        NEW_VERSION = '1.0'
        SERVER_CREDENTIALS = credentials('8a4643cb-9c64-4b2e-a378-17c37f31af22')
        // version defined github cred id specified
    }
    // parameters {

    // }
    stages{
        stage("build"){
            steps{
                echo "build started, building frontend"
                // when {
                //     expression {
                //         BRANCH_NAME == 'master' 
                //     }
                // }
                // echo "building version ${NEW_VERSION}"
                // nodejs('Node-10.19') {
                //     sh 'npm build .'
                // }

            }
        }
        stage("test"){
            steps{
                echo "testing started"
                echo "testing complete"
            }
        }
        stage("deploy"){
            steps{
                echo "deploying on server..."
            }
        }
    }
    post {
        success {
            echo "Pipeline executed Successfully"
        }
        failure {
            echo "Pipeline execution failed"
        }
    }
}  