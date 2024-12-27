pipeline {
    agent any
    stages {
        stage('Clean Workspace') {
            steps {
                deleteDir()  // Clean up the workspace
            }
        }
        stage('Clone Repository') {
            steps {
                // Clone the repository from GitHub, explicitly using the 'main' branch
                git branch: 'main', url: 'https://github.com/uzairsaeedi/empty.git'
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
               sh "cp -r Jenkinsfile assets index.html readme.txt /var/www/html/"

            }
        }
    }
}
