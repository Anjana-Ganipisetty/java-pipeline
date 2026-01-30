pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Compile') {
            steps {
                bat 'javac src\\HelloWorld.java'
            }
        }

        stage('Run') {
            steps {
                bat 'java -cp src HelloWorld'
            }
        }
    }
}
