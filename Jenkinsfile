pipline {
  agent any
  stages {
    stage('gitrepo & clean') {
      steps{
        sh "git clone https://github.com/DTN91/Pipeline.git"
        sh "mvn clean"
      }
    }
    stage('Build'){
      steps{
        sh "mvn install"
      }
    }
  }
}
