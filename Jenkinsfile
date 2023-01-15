pipeline {
  agent any
  tools { 
        maven 'Maven_3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=sonartaken -Dsonar.organization=sonartaken -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=b84e16095ed56f317c10c05f17cc9f1b556cdcdb'
			}
        } 
  }
}
