pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.organization=asgbuggywebappraj -Dsonar.host.url=https://sonarcloud.io -Dsonar.projectKey=asgbuggywebappraj -Dsonar.login=a62867bac064ebc124a8cc44b9f0675f841af507'
			}
        } 
  }
}
