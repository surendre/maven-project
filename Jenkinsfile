pipeline {
    agent any

    tools {
    	maven 'Surendra_Maven'
	
	}


    stages {
            stage('Build') {
                steps {
             		sh 'mvn clean package'
					sh "docker build . -t tomcatwebapp:${env.BUILD_ID}"
	   			}
    		}
    }
}
