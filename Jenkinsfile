pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggy-webapp -Dsonar.organization=asgbuggy-webapp 
		-Dsonar.host.url=https://sonarcloud.io -Dsonar.login=e8fb99b064cdbdcd2a9df46c53a7ae709eb6daee'
		}
        } 
  }
}
