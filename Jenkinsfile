pipeline {
  agent any
  tools { 
        maven 'Maven_3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgnolet7app -Dsonar.organization=asgnolet7app -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=74dcccba36d9c7bc7cd0093ec1c79b42a021da5e'
			}
        } 
  }
}
