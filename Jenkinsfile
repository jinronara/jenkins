pipeline {
  agent {
    node {
      label 'd2ficap1'
    }
    
  }
  stages {
    stage('error') {
      steps {
        parallel(
          "\uBC30\uD3EC\uBAA9\uB85D \uC870\uD68C": {
            sh 'df -g'
            bat(script: '1212.bat', encoding: '121', returnStatus: true, returnStdout: true)
            
          },
          "XML \uC0DD\uC131": {
            bat(script: 'xmlcreate.bat', returnStatus: true, returnStdout: true)
            
          }
        )
      }
    }
  }
  environment {
    ITSM_CLASSPATH = 'ITSM Class Path'
    BIZ = 'CLM'
    TARGET = 'DEV'
  }
}