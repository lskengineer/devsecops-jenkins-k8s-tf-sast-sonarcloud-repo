pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=jenkinsrun -Dsonar.organization=jenkinsrun -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=b92f14d4718afe6fa5a8c793ed68ec7e09a446e0'
			}
        } 
  }
}
