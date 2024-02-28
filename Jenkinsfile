pipeline{
    agent any
    environment{
        TEST="test_value"
        TEST1="test_value1"
    }
        parameters{string (name:"PARAM_STRING",defaultValue:"input_param")

        }
        stages{
            stage('Build'){
                environment{
                    Build_name ="my build"
                }
                steps{
                    sh'''
                    echo $TEST $Build_name
                    sleep 5
                    '''
                }
            }
        stage('Test'){
            steps{
                script{
                echo "${env.TEST}"
            }
            
            }

        }  


        }
}


        
    
    
    
            


        
    