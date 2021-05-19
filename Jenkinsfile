pipeline {
  agent any
  environment {
    PATH = "/Users/c831380/apache-maven-3.6.3/bin/:$PATH"
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
