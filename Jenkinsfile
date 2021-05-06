pipeline {
  agent any
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
