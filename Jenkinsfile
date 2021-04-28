pipeline {
  agent any
  stages {
    stage('Getting Code ') {
      steps {
        git(url: 'https://github.com/faisalfareed26/maven-web-application.git', branch: 'development', credentialsId: 'GitHub_Credentials', poll: true)
      }
    }

    stage('sonarqube report') {
      steps {
        sh '"${mavenHome}/bin/mvn sonar:sonar'
      }
    }

  }
  environment {
    mavenHome = 'tool name : "Maven 3.6.3"'
  }
}