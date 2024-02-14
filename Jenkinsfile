pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp5 -Dsonar.organization=asgbuggywebapp5 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=8d1e5a81a8a068e04ac3f2465ea6b338dbced03b'
		}
        } 
  }
}
