pipeline {
  	agent any
  	stages {
    	stage('Upload to AWS') {
      		steps {
        		withAWS(credentials:'aws-static') { 
		      		s3Upload(file:'index.html', bucket:'udacity-jenkins-pipeline-project', path:'index.html') 
   				} 
    		}
    	}
  	}
}
