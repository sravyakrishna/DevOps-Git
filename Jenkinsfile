pipeline {
   agent {
     label 'nginxslave'
     }
     stages {
       stage ('Checkout') {
           steps {
             node ('nginxslave') {
               checkout scm
             }
            }
         }      
        stage ('NginxDeployment') {
           steps {
              node ('nginxslave') {
                sh 'sudo cp /home/ubuntu/workspace/nginx-pipeline/* /var/www/html/ '
              }
           }
            
        }
              
     }
   
}
   

