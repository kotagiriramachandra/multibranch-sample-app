pipeline {
  agent {jenkins-agent}
  options {
    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeppStr: '5', daysToKeepStr: '', numToKeepStr: '5')
    dsableConcurrentBuilds()
  }
  stages {
    stage {'Hello'}
      steps {
        echo 'Hello Developer'
      }
  }
}
