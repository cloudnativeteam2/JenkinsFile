pipeline 
{
    agent any

    stages 
    {
        
        stage('Build') 
        {
            steps {
                echo 'Build App'
            }
        }
        
        stage('Test') 
        {
            steps {
                echo 'Test App'
            }
        }
        
        stage('Deploy') 
        {
            steps {
                echo 'Deploy'
            }
        }
 
    }

    post
    {
        always
        {
            emailext body: 'Summary', subject: 'Pipeline Status', to: 'cloudNativeTeam2@gmail.com'
        }
    }
}
