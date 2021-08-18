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
                 
                 sh 'sudo -S docker login -u anupbpote -p @Nup_2499'
                 sh 'sudo -S docker build -t anupbpote/myimage6 . '
                 sh 'sudo -S -p @Nup_2499'
                }
            }
     }
    }
