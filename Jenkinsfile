pipeline {
  agent any
  stages {
    stage('Semgrep') {
      steps {
        sh '''echo \'Running semgrep...\'
/usr/local/bin/docker run --rm -v "${PWD}:/src" returntocorp/semgrep --error --config=https://semgrep.dev/p/r2c-CI'''
      }
    }

  }
}