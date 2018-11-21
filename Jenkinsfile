pipeline {
  agent any
  stages {
    stage('BuildP') {
      steps {
        bat 'py menu.py'
      }
    }
    stage('Print') {
      steps {
        echo 'Step 1 Executed Successfully '
      }
    }
  }
}