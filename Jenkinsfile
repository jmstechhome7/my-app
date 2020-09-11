pipeline {
  agent any
  stages {
    stage('getcode') {
      steps {
        git(url: 'https://github.com/jmstechhome7/my-app.git', branch: 'master', changelog: true, poll: true)
      }
    }

    stage('maven') {
      steps {
        sh 'mvn package'
      }
    }

  }
}