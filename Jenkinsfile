pipeline {
    agent any

    tools {
        jdk 'JDK17'
        maven 'Maven'
    }

    stages {

        stage('Checkout') {
            steps {
                git 'https://github.com/PragatiJayaramRathod/ProductInventorySystem.git'
            }
        }

        stage('Build') {
            steps {
                sh 'java -version'
                sh 'mvn clean package'
            }
        }
    }
}
