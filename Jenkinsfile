pipeline {
  agent {
    docker {
      image 'returntocorp/semgrep-agent:v1'
      args '-u root'
    }

  }
  stages {
    stage('Semgrep-agent') {
      steps {
        sh '/root/.local/bin/semgrep --version '
      }
    }

  }
}