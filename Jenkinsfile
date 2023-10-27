pipeline {
    
    agent any
    
    environment {
        gitBranch="${GIT_BRANCH}"
        commitId="${GIT_COMMIT}"
        buildId="${BUILD_ID}"
    }
    
    stages {

        stage('Hello') {
            
            environment {
                employee = "raksha soni"
            }
            
            steps {
                echo 'Hello World'
                echo "My name is ${employee}"
                echo "My name is ${BUILD_ID}"
                echo "buld ID = ${buildId}"
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
            
            // when {
            //     branch 'master'
            // }
            
            // when {
            //     expression {
            //         params.animal == 'lion'
            //     }
            // }
            
            steps {
                echo "Hello World i am deploying"
                echo "My name is ${name}"
                echo "My pet is a ${animal}"
            }
        }
        
        stage('paramters') {
            steps {
                echo "My pet is a ${animal}"
            }
        }
    }

}
