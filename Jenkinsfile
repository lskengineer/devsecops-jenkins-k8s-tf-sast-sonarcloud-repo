pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp -Dsonar.organization=asggbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=b4a31a5eabb2749e86f0355cf1d83c15d069ea0a'
			}
        } 
  }
}
