pipeline{
    agent any
     triggers { cron(*/5 * * * *) }.
        
        
        
        stages{
            stage('checkout'){
                steps{
                    checkout([$class: 'GitSCM',
                    branches: [[name: '*/main']],
                    userRemoteConfigs: [[url: 'https://github.com/Mithunhm5/pipeline_repo.git'
                    credentialsID:'jan_github']]])
                }
            }
        stage('Test'){
            steps{
                sh '''
                ls -lrt
                '''
            }
            
            }

        }  


        }



        
    
    
    
            


        
    