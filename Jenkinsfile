pipeline{
 agent any
  stages{
    stage("Git Checkout"){
       steps{
        checkout scm
       }
      }
     stage ('docker build image') { 
        steps {  
                 sh 'sudo docker login -u anupbpote -p @Nup_2499'
                 sh 'sudo docker build -t anupbpote/myimage6 . '
                }
            }
     }
    }
