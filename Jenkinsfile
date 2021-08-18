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
                 
                        sh 'docker login -u anupbpote -p @Nup_2499'
                        sh 'docker build -t anupbpote/myimage6 . '
                
                       }
                                            }
               stage ('docker tag image'){
                  steps{
                       sh 'docker tag myimage6:latest anupbpote/myimage6:latest'
                       }
                                        }
               stage ('docker push image'){
                  steps{
                       sh 'docker push anupbpote/myimage6:latest'
                       }
   
                       }
       }
    }
