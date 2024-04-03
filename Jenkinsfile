pipeline {
    agent any
    
    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/your-username/your-repository.git'
            }
        }
        stage('Build') {
            steps {
                sh 'Jenkinsfile.sh'
            }
        }
    }
}
