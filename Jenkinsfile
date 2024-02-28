pipeline{
    agent {
        label 'jenkins_slave1'
    }
        stages{
        stage("Build"){
            steps{
                sh 'sleep 5'
                   }
           
        }
    
    
        stage("Test"){

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
    