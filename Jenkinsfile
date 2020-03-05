pipeline {
	
	agent any        
        tools {
            maven 'localmaven'
        }
	stages{
		stage('Build'){

			steps {
                    sh 'mvn clean package'
		    sh ' docker build . -t tomcatwebapp'
			}
		}
	}
}
