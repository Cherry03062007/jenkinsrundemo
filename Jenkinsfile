pipeline {
    agent any 
    stages {
        stage('Clone Repo') { 
            steps {
          sh "export AWS_DEFAULT_REGION=ap-south-1"
          
sh "aws cloudformation create-stack --stack-name myteststack --template-body file://S3Bucket.json --region 'ap-south-1'"
          
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
