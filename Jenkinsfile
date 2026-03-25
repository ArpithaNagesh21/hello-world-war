pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git url: 'https://github.com/ArpithaNagesh21/hello-world-war.git'
            }
        }

        stage('Build') {
            steps {
                sh '''
                  mvn clean package
                  docker build -t hello-war:1.0 .
                '''
            }
        }
    }
}
