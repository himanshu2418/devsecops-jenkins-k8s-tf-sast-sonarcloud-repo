pipeline {
  agent any
  tools { 
        maven 'mvn-3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=adminsec1 -Dsonar.organization=adminsec1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=dd9e59ee15bb87c99a27a3e26562e2d8f52218bc'
			}
        } 
  }
}
