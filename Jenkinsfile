
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main',
                url: 'https://github.com/YOUR_USERNAME/Palindrome-java.git'
            }
        }

        stage('Compile') {
            steps {
                sh 'javac Palindrome.java'
            }
        }

        stage('Execute') {
            steps {
                sh 'java Palindrome 121'
                sh 'java Palindrome 123'
            }
        }
    }
}
