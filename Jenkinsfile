pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecops1-kb -Dsonar.organization=devsecops1-kb -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=6388cfceaadf0f5725a5921b0d8dffb0f4648d53'
			}
        } 
  }
}
