pipeline {
	agent any
    tools {
        go 'Go'
    }
    environment {
        GO111MODULES="on"
    }
	stages {
		stage ('checkout') {
			steps {
				checkout scm
			}
		}
        stage('Compile Go') {
            steps {       
                echo 'GO project'   
                sh 'go build'                                                   

            }
        }
	}// stages
}// pipline