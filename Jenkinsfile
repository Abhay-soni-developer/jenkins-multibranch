pipeline {
    
    agent any
    
    environment {
        gitBranch="${GIT_BRANCH}"
        commitId="${GIT_COMMIT}"
        buildId="${BUILD_ID}"
    }
    
    stages {
        stage('build_docker_image') {
            echo 'Hello World'
            echo "My name is ${gitBranch}"
            echo "My name is ${BUILD_ID}"
            echo "buld ID = ${buildId}"
            echo "branch name = ${GIT_BRANCH}"
        }

        stage('deploy'){
            steps{
                echo "========executing A========"
            }
        }
    }
    
}
