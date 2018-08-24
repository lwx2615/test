pipeline {
  agent any
  stages {
    stage('copy') {
      steps {
        archiveArtifacts(allowEmptyArchive: true, fingerprint: true, artifacts: 'test')
      }
    }
  }
}