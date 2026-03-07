pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
               git 'https://github.com/sejalhule03/javarep.git'
            }
        }
        
        stage('Build') {
            steps {
                echo 'Comipiling in progress'
                bat 'javac Hello.java'
            }
        }
         stage('Executte') {
            steps {
                echo 'Executing....'
                java Hello.java
                bat 'java Hello.java'
            }
        }
     }
}
