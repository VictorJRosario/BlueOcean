pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            sh 'echo "Hello World"'
            sh '''echo "Multiline shell steps works too"
ls -lah'''
          }
        }

        stage('Lint HTML') {
          steps {
            sh 'sh \'tidy -q -e *.html\''
          }
        }

      }
    }

  }
}