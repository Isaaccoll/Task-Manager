pipeline
{
    agent any

    stages 
    {
        stage('CurrentBuild')
        {
            steps 
            {
                sh "pwd"
            }
        }
        stage('Checkout') 
        {
            steps 
            {
               echo 'Checking out the application'
            }
        }
        stage('Build')
        {
            steps {
               echo ' building the application'
                 }
         }
        stage('Test')
        {
            steps
            {
               echo ' testing the application'
                sh 'pytest'
            }
        }
    }
}
