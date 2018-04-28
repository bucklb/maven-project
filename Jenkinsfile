
pipeline {
    agent any
    tools {
        maven 'localMaven'
    }
    stages{	
	    stage('Build'){
		steps {
			echo "Not having any fun!"
			sh 'mvn -version'
			echo "Close to giving up!"
            }
        }
   }
}
