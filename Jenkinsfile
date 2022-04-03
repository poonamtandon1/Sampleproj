pipeline { 
  
   agent any

   stages {
   
     stage('Install Dependencies') { 
        steps { 
           sh 'echo "installing dependencies"'
        }
     }
     
     stage('Test') { 
        steps { 
           sh 'echo "testing application..."'
        }
      }

 	stage('Build') { 
        steps { 
           sh 'echo "building application..."'
        }
      }

	if(env.BRANCH_NAME == 'develop'){
     	stage("Develop"){
        	sh 'echo "branch develop..."'
        }
     }

	if(env.BRANCH_NAME == 'master'){
     		stage("Master"){
        	sh 'echo "branch master..."'
        }
     }

         stage("Deploy application") { 
         steps { 
           sh 'echo "deploying application..."'
         }

     }
  
   	}

   }
