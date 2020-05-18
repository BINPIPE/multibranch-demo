pipeline{
    agent any
    stages{
        stage("Deploy Dev"){
            when {
                // This works only in multi branch pipeline
                branch 'development'
            }
            steps{
                echo "Deploying to Dev environment"
            }
        }
        stage("Deploy Staging"){
            when {
                branch 'staging'
            }
            steps{
                echo "Deploying to Staging environment"
            }
        }

        stage("Deploy Prod"){
            when {
                branch 'master'
            }
            steps{
                echo "Deploying to Prod environment"
            }
        }
    }
}
