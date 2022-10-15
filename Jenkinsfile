pipeline {
    agent { label 'OPENJDK-11-JDK'}
    stages {
        stage {
            steps('vpc') {
                sh """aws ec2 create-vpc
                    --cidr-block "10.0.0.0/16"""
            }
        }
    }
}