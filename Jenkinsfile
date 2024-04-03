pipeline {
    agent any
    
    stages {
        stage('Clone Repository') {
            steps {
                script {
                    // Checkout the code from SCM
                    checkout scm
                }
            }
        }
        stage('Build') {
            steps {
                script {
                    // Execute build script
                    sh './CST_Play/Jenkinsfile.sh'
                }
            }
        }
    }
    post {
        always {
            // Cleanup steps, if necessary
        }
        success {
            echo 'Pipeline completed successfully'
        }
        failure {
            echo 'Pipeline failed'
            // You can add additional actions for failure handling here
        }
    }
}

