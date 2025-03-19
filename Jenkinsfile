pipeline {
  agent {lable 'linux'}
  options {
    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeppStr: '5', dayToKeepStr: '', numToKeepStr: '5')
    dsableConcurrentBuilds()
    }
  stages {
    stage {'Hello')
      steps {
        echo 'Hello Developer'
      }
    }
  }
}
