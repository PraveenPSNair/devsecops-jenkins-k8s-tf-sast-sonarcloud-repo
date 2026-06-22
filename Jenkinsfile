pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=myapptest -Dsonar.organization=myapptest -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=7bb1e43b3156f776fe88a181c87d90e7e20e7904'
			}
        } 
  }
}
