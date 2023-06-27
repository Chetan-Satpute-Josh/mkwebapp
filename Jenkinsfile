pipeline 
{
    agent any 
    tools 
    {
        nodejs 'node'
    }

    stages 
    {
        stage('Checkout') 
        {
            steps 
            {
                checkout scm
            }
        }

        stage('Build') 
        {
            steps 
            {
                sh 'npm install'
                sh 'npm run build'
                sh 'ls'
            }
        }
        stage('Test') 
        {
            steps 
            {
                echo 'Testing...'
            }
        }
        stage('Deploy') 
        {
            steps 
            {
                echo 'Deploying....'
            }
        }
    }
}

