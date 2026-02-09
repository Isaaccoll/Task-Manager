pipeline {
    agent any
    environment {
        NEW_VERSION = '1.3.0'
        SERVER_CREDENTIALLS = credentials('')
    }
    stages {
        stage('CurrentBuild') {
            steps {
        
                sh "pwd"
            }
        }
        stage('Checkout') {
            steps {
               echo 'Checking out the application'
            }
        }
        stage('Build')
        {
            steps {
               echo ' building the application'
               echo "Building version ${NEW_VERSION}"
                 }
         }
        stage('Test')
        {
            steps {
               echo ' testing the application'
                sh 'pytest'
                 }
         }
    }
    post {
        always {
            // 
        }
        success {
            
        }
        failure {
            
        }
    }
    
}
