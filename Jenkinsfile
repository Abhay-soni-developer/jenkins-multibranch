pipeline {
    
    agent any
    
    environment {
        gitBranch="${GIT_BRANCH}"
        commitId="${GIT_COMMIT}"
        buildId="${BUILD_ID}"
    }
    
    stages {


        stage('approve') {

            input { 
                message "should we continue"
            }
            
            steps {
                echo "this is confirmation stage"
            }
        }

        
        stage('Hello') {
            
            environment {
                employee = "raksha soni"
            }
            
            steps {
                echo 'Hello World'
                echo "My name is ${employee}"
                echo "My name is ${BUILD_ID}"
                echo "buld ID = ${buildId}"
                echo "build branch = ${gitBranch}"
                echo "my commit ID = ${commitId}"
                // echo "${DOCKER_CREDS_USR}"
                
                echo "${PATH}"
                
                // nodejs("local-node") {
                //     sh "node --version"
                // }
                // sh "node --version"
                // sh "docker version"
            }
        }
        
        stage('production') {
            
            
            steps {
                echo "Hello World i am deploying"
            }
        }
        
        stage('paramters') {
            steps {
                echo "My pet is a Abhay"
            }
        }
    }

}
