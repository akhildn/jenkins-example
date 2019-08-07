pipeline {
  agent any
  stages {
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
