pipeline {
  options {
    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')
    disableConcurrentBuilds()
  }
  stages {
    stage ('Hello') {
      steps {
        echo 'Hello Developer'
      }
    }
    stage ('Dev code') {
      when {
        branch "dev-*"
      }
      steps {
        echo "Dev changes are done"
      }
    }	
  }
}
