pipeline {
    agent any

    tools {
        maven 'Maven_3.8.7'
        jdk 'JDK_17'
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/SHASHANK9060/TOMCAT.git'
            }
        }

        stage('Build WAR') {
            steps {
                sh 'mvn clean package'
            }
        }

    }
}
