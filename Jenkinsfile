pipeline {
  agent any
  stages {
    stage('UploadtoAWS') {
      steps {
        withAWS(region:'us-east-1' credentials:'AKIAZEKYXXENPSJP2RKC', 't7sX1MJfx3P7iBHgP3OrDHr+bOp/qdil22dsdJIT') {
          s3Upload(file:'index.html', bucket:'smiddleycicd' path:'https://smiddleycicd.s3.amazonaws.com/index.html')
        }
       }
     }
   }
}
