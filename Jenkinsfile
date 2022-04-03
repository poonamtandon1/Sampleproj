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

    stage('develop-test') {
       when {
          branch 'develop'
       }
       steps {
          sh  'echo "triggered by develop"'
      }
  }

stage('master') {
       when {
          branch 'master'
       }
       steps {
          sh  'echo "triggered by master"'
      }
  }

         stage("Deploy application") { 
         steps { 
           sh 'echo "deploying application..."'
         }

     }
  
   	}

   }
