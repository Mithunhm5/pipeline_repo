pipeline{
    agent none
        
        stages{
        stage("Build"){
          agent {
            label 'slave1'
          }  
          steps{
                sh 'sleep 5'
                   }
           
        }
    
    
        stage("Test"){
          agent any
            steps{
                sh '''
                #!/bin/bash
                ls
                sleep 5
                '''
                    }
        }
            


        }
}
    