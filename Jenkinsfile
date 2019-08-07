pipeline {
  agent any
  stages {
    stage('build'){
      steps{
        sh 'echo "hello udacity"'
        sh '''
            echo "Multiline shell steps works too"
            ls -lah
            '''
      }
    }
  }
}
