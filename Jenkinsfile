pipeline {
    agent { label 'OPENJDK-11-JDK'}
    stages {
        stage {
            steps {
                sh 'aws ec2 create-vpc --cidr-block "192.168.0.0/16" '
            }    
        }
    }
}
