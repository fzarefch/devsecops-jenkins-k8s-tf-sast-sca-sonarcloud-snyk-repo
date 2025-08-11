pipeline {
  agent any
  tools { 
    maven 'Maven_3.8.7'
  }
  stages {
    stage('CompileandRunSonarAnalysis') {
      steps {
        sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=aasgbuggywebapp1994 -Dsonar.organization=asgbuggywebapp1994 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=d7cab012794744ea30c6de6a3a9cfdda2f4813db'
      }
    }
  }
}
