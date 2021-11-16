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
	           }
		          
		  
	     
	     }
