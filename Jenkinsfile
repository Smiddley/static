pipeline {
  agent any
  stages {
    stage('UploadtoAWS') {
      steps {
        withAWS(region:'us-east-1') {
          s3Upload(file:'index.html', bucket:'smiddleycicd', path: 'https://github.com/Smiddley/static/index.html')
        }
       }
     }
   }
}
