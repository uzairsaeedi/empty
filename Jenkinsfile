pipeline {
    agent any
    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/uzairsaeedi/empty.git'
            }
        }
        stage('Build') {
            steps {
                echo 'No build steps required for static website.'
            }
        }
        stage('Test') {
            steps {
                echo 'No tests required for static website.'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying static website...'
                // Ensure the deployment path matches your environment. Adjust `/var/www/html/` to your server's actual web root directory if different.
                sh 'cp -r * /var/www/html/'
            }
        }
    }
}