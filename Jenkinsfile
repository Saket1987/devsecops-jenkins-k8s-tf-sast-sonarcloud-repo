pipeline {
  agent any
  tools { 
        maven 'Maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=saketasgbuggywebapp -Dsonar.organization=saketasgbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=d050691cf7bac81f87db38d4a751323ec95d73be'
			}
        } 
  }
}
