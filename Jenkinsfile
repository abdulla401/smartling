pipeline {
  agent any
  stages {
    stage('myStage'){
      steps {
        sh 'ls -la'
      }
    }
    stage('Build') {
      steps {
        sh 'git diff HEAD~1'
      }
    }
    stage('Checkout') {
            steps {
                lastChanges format:'SIDE',matching: 'WORD', specificRevision: "${REV}"
            }
        }
     stage('Builds2222') {
      steps {
        sh 'ls -ltr'
      }
    }
  }
}
