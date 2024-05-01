pipeline {
    agent any

    stages {
        stage('Hello World') {
            steps {
                bat 'javac HelloWorld.java'
                bat 'java HelloWorld'
            }
        }
        stage('Hello Wipro') {
            steps {
                bat 'javac HelloWipro.java'
                bat 'java HelloWipro'
            }
        }
        stage('Hello Jenkins') {
            steps {
                bat 'javac HelloJenkins.java'
                bat 'java HelloJenkins'
            }
        }
    }

    post {
        always {
            script {
                // Clean up
                deleteDir()
            }
        }
    }
}
