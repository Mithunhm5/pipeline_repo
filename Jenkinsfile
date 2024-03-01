pipeline {
    agent any

    triggers {
        cron(*/5 * * * *)
    }

    stages {
        stage('Checkout') {
            steps {
               checkout([$class: 'GitSCM', branches: [[name: '*/main']],
                          userRemoteConfigs: [[url: 'https://github.com/Mithunhm5/pipeline_repo.git'
                          credentialsId: 'jan_github' ]]])
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

