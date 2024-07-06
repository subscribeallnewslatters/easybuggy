pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=grabassignment -Dsonar.organization=grabassignment -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=ec85cb53eb4c6a4a33be826fe11ef81a618ad107'
			}
        } 
  }
}
