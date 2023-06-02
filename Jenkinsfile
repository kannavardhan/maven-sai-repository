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
