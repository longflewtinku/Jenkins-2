pipeline {
    agent { label 'OPENJDK-11-JDK'}
    stages {
        stage {
            steps('vpc') {
                sh 'aws ec2 create-vpc `
                    --cidr-block "10.0.0.0/16" `
                    --tag-specification "ResourceType=vpc,Tags=[{Key=Name,Value=MyVpc}]"'
            }
        }
    }
}