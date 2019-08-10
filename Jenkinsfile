pipleine {
  agent any
  stages {
    stage('Upload to AWS.') {
      steps {
        withAWS(region:'us-east-2',credentials:'aws-static') { 
		      s3Upload(bucket: 'udacity-jenkins-pipeline-project', workingDir:'.', includePathPattern:'*.html'); 
		    } 
	    }
    }
  }
}
