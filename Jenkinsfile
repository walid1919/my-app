 pipeline
   {

		agent any
		  stages {
                    stage("build"){ 
                     
                        steps{ 

                           script{
                             sh "ansible-playbook /home/walid/CD/my-app/ansible/build.yml -i /home/walid/CD/my-app/ansible/inventory/host.yml" 
                             }

                             }
                 
                         
  }


           stage('docker'){
                  steps{
                     script{
                            sh "ansible-playbook /home/walid/CD/my-app/ansible/docker.yml -i /home/walid/CD/my-app/ansible/inventory/host.yml"
                     }
                  }
              }
              stage('Push to DockerHub'){
                  steps{
                     script{
                            sh "ansible-playbook /home/walid/CD/my-app/ansible/docker-registry.yml -i /home/walid/CD/my-app/ansible/inventory/host.yml"
                     }
                  }
              }
	           }
		          
		  
	     
	     }
