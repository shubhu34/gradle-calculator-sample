pipeline
{
	agent any
	stages
	{
		stage ('scm checkout')
		{
			steps { git branch: 'master', url: 'https://github.com/shubhu34/gradle-calculator-sample/' }
		}

		stage ('run-gradle-command-to-build-and-geneate-artifacts')
		{
			steps { sh './gradlew clean'
				sh './gradlew assemble'
				sh './gradlew build'
				sh './gradlew jar'
				}
		}

	}

}