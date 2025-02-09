pipeline {
    agent any
    
    stages {
        stage('Install Apache2') {
            steps {
                script {
                    // Run the command to install Apache2
                    sh 'sudo apt update'
                    sh 'sudo apt install -y apache2'
                }
            }
        }
    }
}
