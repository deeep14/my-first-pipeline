pipeline
{
    agent any
    stages
    {
        stage("Build")
        {
            steps
            {
                echo "Building"
            }
        }
        stage("Test")
        {
            steps
            {
                echo "Testing"
            }
        }
        stage("Deploy")
        {
            when
            {
                expression
                {
                    env.BRANCH_NAME == "master"
                }
            }
            steps
            {
                echo "Deploying"
            }
        }
   }
}
