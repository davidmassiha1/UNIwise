pipeline {
    agent any
    tools {
        go 'go1.19'
    }
    environment {
        GO114MODULE = 'on'
        CGO_ENABLED = 0 
        GOPATH = "${JENKINS_HOME}/jobs/${JOB_NAME}/builds/${BUILD_ID}"
    }
    
      stages {  
        stage('Build') {
            steps {
                echo 'Compiling and building'
                sh 'go build main.go'
            }
        }

       
        
    }
}
    
