pipeline {
    agent any
    
    stages {
        stage('Install Apache2') {
            steps {
                script {
                    // Run the command to install Apache2
                    sh 'apt update'
                    sh 'apt install -y apache2'
                }
            }
        }
    }
}
