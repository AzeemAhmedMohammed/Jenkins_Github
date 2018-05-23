pipeline {
    agent any

    stages {
        stage('Test') {
            steps {
                /*  returns non-zero on test failures,
                * using  to allow the Pipeline to continue nonetheless
                */
                sh 'make check || true' 
                junit '**/target/*.xml' 
            }
        }
    }
}
