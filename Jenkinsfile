pipeline {
  agent any
  stages {
    stage('Git') {
      steps {
        git(url: 'https://github.com/BoondockRiley/SQL', branch: 'main', credentialsId: 'BR1', poll: true)
        echo 'Done'
        script {
          // Run bash command using specific bash executable
          bat '"C:\\Program Files\\Git\\bin\\bash.exe" -c "PWD"'
          bat '"C:\\Program Files\\Git\\bin\\bash.exe" -c "liquibase --version"'
          bat '"C:\\Program Files\\Git\\bin\\bash.exe" -c "liquibase flow"'
        }
      }
    }
  }
}
