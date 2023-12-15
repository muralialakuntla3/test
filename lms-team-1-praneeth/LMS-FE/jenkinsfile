pipeline {
    agent any
    stages {
        stage ('Checkout') {
            steps {
                // Checkout the source code from your version control system (e.g., Git)
                sh 'echo checkout SCM'
            }
        }
        stage ('remove container') {
            steps {
                sh 'sudo docker container rm -f fe'
            }
        }
        stage ('Docker Build') {
            steps {
                sh 'cd lms-team-1-praneeth/LMS-FE && sudo docker build -t frontend .'
            }
        }
        stage ('container') {
            steps {
                sh 'sudo docker run -dt --name fe -p 80:80 frontend'
            }
        }
    }
}
