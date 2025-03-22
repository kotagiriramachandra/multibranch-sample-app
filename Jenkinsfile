pipeline {
  agent any
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
    stage ('Data') {
      steps {
        echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
	echo "Build no ${env.BUILD_NUMBER}"
	echo "Build tag ${env.BUILD_TAG}"
	echo "Exceutor no ${env.EXECUTOR_NUMBER}"
	echo "java home ${env.JAVA_HOME}"
	echo "Job name ${env.JOB_NAME}"
	echo "Node name ${env.NODE_NAME}"
	echo "Workspace ${env.WORKSPACE}"
      }
    }
  }
}
