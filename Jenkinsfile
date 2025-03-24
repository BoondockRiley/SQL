pipeline {
  agent any
  stages {
    stage('Git') {
      steps {
        git(url: 'https://github.com/BoondockRiley/SQL', branch: 'main', credentialsId: 'github-token2', poll: true)
        echo 'Done'
      }
    }

  }
}