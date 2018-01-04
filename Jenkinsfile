pipeline{
    agent any
    stages{
        stage ('build'){
            steps{
                echo 'Build number is: ${env.BUILD_NUMBER}'
		echo 'My branch is: ${env.BRANCH_NAME}'
            }
        }
    }
}
