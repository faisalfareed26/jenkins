pipeline {
  agent any
  stages {
    stage('Getting Code ') {
      steps {
        git(url: 'https://github.com/faisalfareed26/maven-web-application.git', branch: 'development', credentialsId: 'GitHub_Credentials', poll: true)
      }
    }

  }
}