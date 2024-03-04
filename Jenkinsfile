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


        }
    }
}
}
    