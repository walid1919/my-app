   pipeline
   {

		agent any
		  stages {
		      stage('Pull') {
			   steps{
			      script{
				  checkout([$class: 'GitSCM', branches: [[name: '*/master']],
				      userRemoteConfigs: [[
					  credentialsId: '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',
					  url: 'https://github.com/walid1919/CD.git']]])
			      }
		          }
		     }
	     }
	     }
