pipeline {
    agent any
    stages{
        stage('Checkout'){
            steps{
                withCredentials([usernamePassword
                (credentialsId:'slave_ssh',usernameVariable:'USER',passwordVariable:'PASS')])
            {
                echo"$USER$PASS"
                sh'''
                echo "$USER  $PASS"
                '''

            }

        withCredentials([string
                (credentialsId:'test_up',usernameVariable:'USER',)])
            {
                echo"$USER"
                sh'''
                echo "$USER"
                '''



            }
        }
    }
}

    