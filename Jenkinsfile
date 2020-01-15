pipeline {
    agent any
    stages {
        stage('Upload to AWS'){
            withAWS(credentials:'aws-static') {
              s3Upload(file:'index.html', bucket:'ecme-p3-udacity', path:'index.html')
            }
        }
    }
}
