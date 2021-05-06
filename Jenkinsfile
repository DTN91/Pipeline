pipeline {
  agent any
 # node {
  #  System. setProperty ( "org.jenkinsci.plugins.durabletask.BourneShellScript.HEARTBEAT_CHECK_INTERVAL" , "3800" )
  stages {
    stage('clean') {
      steps{
        sh "mvn clean"
      }
    }
    stage('Build'){
      steps{
        sh "mvn install -DskipTests=true"
      }
    }
  }
#  }
}
