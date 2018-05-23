pipeline {
    agent any

    stages {
 New_branch1
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'

        stage('Test') {
            steps {
                /*  returns non-zero on test failures,
                * using  to allow the Pipeline to continue nonetheless
                */
                sh 'make check || true' 
                junit '**/target/*.xml' 
master
            }
        }
    }
}
