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
  }
}