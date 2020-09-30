pipeline {
    agent any
    stages {
        stage ('GitCheckout Stage') {
            steps {
                sh "git checkout development"
            }
        }

        stage ('Testing Stage') {
            steps {
                sh './test.sh'
            }
        }

        stage ('Deployment Stage') {
            steps {
                sh './sample.sh'
            }
        }
    }
}