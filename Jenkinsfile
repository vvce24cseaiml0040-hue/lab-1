pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                echo 'Checking out source code'
            }
        }

        stage('Compile') {
            steps {
                echo 'Compiling Java program'
                bat 'javac hello.java'
            }
        }

        stage('Run') {
            steps {
                echo 'Executing Java program'
                bat 'java hello'
            }
        }
    }

    post {
        success {
            echo 'Build Successful!'
        }

        failure {
            echo 'Build Failed!'
        }
    }
}
