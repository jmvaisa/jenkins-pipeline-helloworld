pipeline {
  agent any 
  stages {
    stage('Build') {
      steps {
        sh 'echo "Hello World"'
        sh '''
                  echo "Multiline shell steps works too"
                  ls -lah
               '''
      }
    }
    stage('Lint HTML') {
      steps {
          sh 'echo "Check the html using tidy"'
          sh 'tidy -q -e *.html'
      }
    }
  }
}