pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.organization=asgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.projectKey=asgbuggywebapp-key_asgbuggywebapp -Dsonar.login=207e925fbe80a5818378108095d4abc087f2a269'
			}
        } 
  }
}
