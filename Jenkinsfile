pipeline {
    agent any
    stages {
        stage('NPM INSTALL') { 
            steps {
                sh 'npm install' 
            }
        }
        stage('Build') { 
            steps {
                sh 'npm run build' 
            }
        }
        stage('Deploy to NGINX') { 
            steps {
                sh 'sudo cp -r build/. /var/www/html/react' 
            }
        }
    }
}