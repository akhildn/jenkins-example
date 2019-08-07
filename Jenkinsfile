pipeline {
  agent any
  stages {
    stage('Lint HTML.'){
      steps{
        tidy -q -e *.html
      }
    }
    stage('Upload to AWS.'){
      steps{
        sh 'echo "hello udacity"'
        withAWS(credentials:'aws-static') {
            // do something
          s3Upload(file:'index.html', bucket:'anayabu-s3-jenkins-static')
        }
      }
    }
  }
}
