pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbwa -Dsonar.organization=asgbwa -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=b7914cb8a98c47125832feec2cd2e65e329e146f'
			}
        } 
  }
}
