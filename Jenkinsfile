pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopsbuggyweb -Dsonar.organization=devsecopsbuggyweb -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=19e799da3c7f5eb053e19d40ef26761f3a68678b'
			}
        } 
  }
}
