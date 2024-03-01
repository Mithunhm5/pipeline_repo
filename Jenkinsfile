pipeline {
    agent any

    triggers {
        cron(*/5 * * * *)
    }

    stages {
        stage('Checkout') {
            steps {
                checkout([
                    'GitSCM',
                    branches: [[name: '*/master']],
                    userRemoteConfigs: [[url: 'https://github.com/Mithunhm5/pipeline_repo.git']],
                    credentialsId: 'jan_github' // Corrected spelling
                ])
            }
        }

        stage('Test') {
            steps {
                sh '''
                    ls -lrt
                ''' // Added semicolon for consistency
            }
        }
    }
}
