pipeline {
  agent any
  environment {
    PATH = "/opt/maven381/bin/:$PATH"
  }
  stages {
    stage('clean') {
      steps{
        git "https://github.com/DTN91/Pipeline"
        sh "mvn clean"
      }
    }
    stage('Build'){
      steps{
        sh "mvn install -DskipTests=true"
      }
    }
  }
}
