pipeline {
  agent any
  stages {
    stage('BuildP') {
      steps {
        bat(script: 'py Menu.py', returnStatus: true)
      }
    }
    stage('Print') {
      steps {
        echo 'Step 1 Executed Successfully '
      }
    }
    stage('ToscaScript') {
      steps {
        bat(script: '"C:\\Program Files (x86)\\TRICENTIS\\Tosca Testsuite\\ToscaCI\\Client\\ToscaCIClient.exe" -m distributed -t junit -r "C:\\Users\\vengurah\\.jenkins\\workspace\\DevOpsToolChain\\Reports\\Result.xml"', returnStatus: true, returnStdout: true)
      }
    }
  }
}