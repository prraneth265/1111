pipeline {
    agent any
    stages {
        stage('Checkout Confirmation') {
            steps {
                echo "Building branch: ${env.BRANCH_NAME}"
                sh 'ls -la'
            }
        }
        stage('Deploy to Production') {
            when {
                branch 'main'
            }
            steps {
                echo 'This only runs on the main branch!'
            }
        }
    }
}
