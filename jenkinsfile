pipeline {
    agent any
    
    stages {
        stage('Hello World') {
            steps {
                script {
                    bat 'python hello_world.py'
                }
            }
        }
        stage('Hello Wipro') {
            steps {
                script {
                    bat 'python hello_wipro.py'
                }
            }
        }
        stage('Hello Jenkins') {
            steps {
                script {
                    bat 'python hello_jenkins.py'
                }
            }
        }
    }
    
    post {
        always {
            script {
                // Archive artifacts if needed
                archiveArtifacts artifacts: '**/*.py'
            }
        }
        success {
            echo 'Pipeline executed successfully!'
        }
        failure {
            echo 'Pipeline execution failed!'
        }
    }
}
