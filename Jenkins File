pipeline
{
    agent any
    stages
    {
        stage("Checkout Source")
        {
            agent any
            steps
            {
                git 'https://github.com/Sharat2712/webapp1.git'
            }
        }
        stage ('Compile')
        {
            agent any
            steps
            {
                sh 'mvn compile'
            }
        }
        stage ('Test Step')
        {
            agent any
            steps
            {
                sh 'mvn test'
            }
        
        }
        stage ('Package Project')
        {
            agent any
            steps
            {
                sh 'mvn package'
            }
        }
    }
}
