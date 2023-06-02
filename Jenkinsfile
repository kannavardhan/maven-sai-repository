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
 stage('SonarQube analysis') {
//    def scannerHome = tool 'SonarScanner 4.0';
        steps{
        withSonarQubeEnv('sonarqube-9.2.4') { 
        // If you have configured more than one global server connection, you can specify its name
//      sh "${scannerHome}/bin/sonar-scanner"
        sh "mvn sonar:sonar"
    }
        }
        }
