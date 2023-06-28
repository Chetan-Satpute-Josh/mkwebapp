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
                sh 'pwd'
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
                // ansiblePlaybook(credentialsId: '/home/ubuntu/.ssh/private_key', inventory: '/home/ubuntu/inventory.yaml', playbook: '/home/ubuntu/playbook.yaml')        
                sh 'pwd'
                sh 'whoami'
                sh 'ansible-playbook playbook.yml -i inventory.yml'
            }
        }
    }
}

