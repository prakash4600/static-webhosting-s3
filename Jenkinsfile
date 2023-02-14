pipeline {
    agent any
    stages {
        stage('deploy') {
            steps {
              sh "aws configure set region = 'eu-west-1' " 
              sh "aws configure set aws_access_key_id = 'AKIA43CCP6Z46PZT4PBJ' "  
              sh "aws configure set aws_secret_access_key = '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' "
              sh "aws s3 cp Code/index.html s3://my-static-bucket-jenkins"
            }
        }
    }
}
