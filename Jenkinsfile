pipeline {
    agent any

    tools {
        jdk 'jdk-17'
    }

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/saiteja-adapa-2909/java-timestamp.git'
            }
        }

        stage('Compile') {
            steps {
                sh 'javac TimestampPrinter.java'
            }
        }

        stage('Run') {
            steps {
                sh 'java TimestampPrinter'
            }
        }
    }
}