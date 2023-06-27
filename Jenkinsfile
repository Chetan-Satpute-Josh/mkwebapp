pipeline 
{
    agent any 
    tools 
    {
        node 'node'
    }

    stages 
    {
        stage('Build') 
        {
            steps 
            {
                sh 'node --version'
            }
        }
        stage('Test') 
        {
            steps 
            {
                echo 'Testing..'
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

