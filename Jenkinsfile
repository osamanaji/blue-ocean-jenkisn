pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/osamanaji/blue-ocean-jenkisn.git', branch: 'master', credentialsId: 'bf75e321-78e0-4cdd-b25f-ba02ffd21d00')
      }
    }

    stage('validate') {
      steps {
        sh 'mvn validate'
      }
    }

    stage('build') {
      steps {
        sh 'mvn complie'
      }
    }

  }
}