pipeline {
    agent any
    stages{
        stage('Cread'){
            steps{
                withCredentials([usernamePassword
                (credentialsId:'test_up',usernameVariable:'USER',passwordVariable:'PASS')])
            {
                echo"$USER$PASS"
                sh'''
                echo "$USER  $PASS"
                '''

            }

               withCredentials([string
                (credentialsId:'slave_ssh',usernameVariable:'USER',)])
            {
                echo"$USER"
                sh'''
                echo "$USER"
                '''
            }
        }
    }
}
}
    