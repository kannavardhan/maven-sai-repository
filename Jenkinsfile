node('built-in') 
{
    stage('Continuous Download') 
	{
    git 'https://github.com/kannavardhan/maven-sai-repository.git'
	}
    stage('Continuous Build') 
	{
    script: 'mvn package'
	}
}
 stage('SonarQube Analysis') {
            steps {
                // Run SonarQube scanner
                // Make sure you have SonarQube scanner installed and configured
                // Example:
                // withSonarQubeEnv('SonarQube Server') {
                //     sh 'sonar-scanner'
                // }
            }
        }
