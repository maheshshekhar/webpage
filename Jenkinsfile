pipeline{
    agent Jenkins
    stages{
        stage ('build'){
            steps{
                echo "Build number is: ${env.BUILD_NUMBER}"
		echo "My branch is: ${env.BRANCH_NAME}"
            }
        }

	stage ('tagging'){
	    steps{
		echo 'Tagging the release'
		sh "git tag ${env.BUILD_NUMBER}"
		sh "git push origin ${env.BUILD_NUMBER}" 
	   }
	}
    }
}
