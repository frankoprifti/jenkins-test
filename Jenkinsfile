pipeline {
    stages {
        stage('NPM INSTALL') { 
            steps {
                sh 'npm install' 
            }
        }
    },
    stages {
        stage('Build') { 
            steps {
                sh 'npm run build' 
            }
        }
    },
    stages {
        stage('Serve') { 
            steps {
                sh 'npx serve -s build' 
            }
        }
    },
}