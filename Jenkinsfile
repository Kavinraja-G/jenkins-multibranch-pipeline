pipeline {
    agent any
    stages {
        stage ('GitCheckout Stage') {

            steps {
                sh "git checkout master"
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