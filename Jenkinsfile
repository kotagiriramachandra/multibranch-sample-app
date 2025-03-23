pipeline {
  agent { lable 'Windows' }
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
	echo "Brach name ${env.BRANCH_NAME}"
	echo "Change id ${env.CHANGE_ID}"
	echo "Change url ${env.CHANGE_URL}"
	echo "Change title ${env.CHANGE_TITLE}"
	echo "Change author ${env.CHANGE_AUTHOR}"
	echo "Change author display name ${env.CHANGE_AUTHOR_DISPLAY_NAME}"
	echo "Change author email ${env.CHANGE_AUTHOR_EMAIL}"
	echo "Change target ${env.CHANGE_TARGET}"
	echo "Change branch ${env.CHANGE_BRANCH}"
	echo "Change fork ${env.CHANGE_FORK}"
	echo "Tag name ${env.TAG_NAME}"
	echo "Job display url ${env.JOB_DISPLAY_URL}"
	echo "Run display url ${env.RUN_DISPLAY_URL}"
	echo "Node labels ${env.NODE_LABELS}"
	echo "Build url ${env.BUILD_URL}"
	echo "Job url ${env.JOB_URL}"
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
