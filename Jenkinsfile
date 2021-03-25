pipeline {
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
        stage('Serve') { 
            steps {
                sh 'npx serve -s build' 
            }
        }
    },
}