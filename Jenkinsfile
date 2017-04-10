pipeline {
  agent {
    node {
      label 'd2ficap1'
    }
    
  }
  stages {
    stage('error') {
      steps {
        sh 'df -g'
      }
    }
  }
  environment {
    ITSM_CLASSPATH = 'ITSM Class Path'
    BIZ = 'CLM'
    TARGET = 'DEV'
  }
}