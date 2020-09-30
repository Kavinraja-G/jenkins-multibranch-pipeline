pipeline {
    agent any
    stages {
        stage ('GitCheckout Stage') {

            steps {
                withMaven(maven : 'maven_3_5_0') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {
            steps {
                sh 'test'
            }
        }

        stage ('Deployment Stage') {
            steps {
                sh 'sample'
            }
        }
    }
}