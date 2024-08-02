pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappraezon -Dsonar.organization=asgbuggywebappraezon -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=1cc2143703da2f6a000facf8727c484101a82c77'
			}
        } 
  }
}
