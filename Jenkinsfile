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
        
        stage('Check Apache Access Log for Errors') {
            steps {
                script {
                    // Run the command to check the Apache access log for 4xx and 5xx HTTP status codes
                    sh 'cat /var/log/apache2/access.log | grep -E \'HTTP/1.1" (4|5)[0-9][0-9]\''
                }
            }
        }
    }
}