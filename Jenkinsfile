pipeline {
  agent any
  stages {
    stage('copy') {
      parallel {
        stage('copy') {
          steps {
            archiveArtifacts(allowEmptyArchive: true, fingerprint: true, artifacts: 'test')
          }
        }
        stage('test') {
          steps {
            build(propagate: true, job: 'test')
          }
        }
        stage('retest') {
          steps {
            build(propagate: true, job: 'test')
          }
        }
      }
    }
    stage('scp') {
      steps {
        sh 'echo ""'
      }
    }
    stage('jieya') {
      steps {
        timestamps()
      }
    }
    stage('bushu') {
      steps {
        build(propagate: true, job: 'test')
      }
    }
    stage('wancheng') {
      steps {
        dir(path: '/')
      }
    }
  }
}