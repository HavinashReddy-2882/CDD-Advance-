pipeline {
    agent any

    stages {

        stage('Check Files') {
            steps {
                bat 'dir'
            }
        }

        stage('Compile Java') {
            steps {
                bat 'javac Add.java'
            }
        }

        stage('Run Java Program') {
            steps {
                bat 'java Add'
            }
        }
    }

    post {
        success {
            echo 'BUILD SUCCESSFUL'
        }
        failure {
            echo 'BUILD FAILED'
        }
    }
}
