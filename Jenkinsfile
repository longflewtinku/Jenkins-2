pipeline {
    agent { label 'OPENJDK-11-JDK'}
    stages {
        stage('vpc') {
            steps {
                sh 'aws ec2 create-vpc --cidr-block "10.10.0.0/16" --region "ap-south-1" --tag-specification "ResourceType=vpc,Tags=[{Key=Name,Value=mumbaiVpc}]"'
            }
        }
    }
}