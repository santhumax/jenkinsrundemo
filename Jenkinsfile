pipeline {
    agent any 
    stages {
        stage('Clone Repo') { 
            steps {
          sh "export AWS_DEFAULT_REGION=eu-east-1"
          
sh "aws cloudformation create-stack --stack-name myteststack --template-body file://S3Bucket.json --region 'eu-east-1'"
          
          }
        }
        stage('Test') { 
            steps {
                sh "ls"
            }
        }
        stage('Deploy') { 
            steps {
               sh "ls"
            }
        }
    }
}
