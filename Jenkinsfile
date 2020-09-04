pipeline {
   agent {
     label 'nginx'
     }
     
     stages {
       stage ('Checkout') {
           steps {
             node ('nginx') {
               checkout scm
             }
            }
       
       }      
        stage ('NginxDeployment'){
           steps {
              node ('nginx'){
                sh 'sudo cp /home/ubuntu/workspace/Project-gitPipeline/* /var/www/html/ '
     
              
              }
           }
            
        }
              
     }
              
   
   

