pipeline {
    agent any 
    stages {
        stage('Clone Repo') { 
            steps {
          sh "export AWS_DEFAULT_REGION=eu-west-1"
          
sh "aws cloudformation create-stack --stack-name mysantstack --template-body file://S3Bucket.json --region 'eu-west-1'"
          
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
