pipeline {
  agent any
  stages {
    stage('Pre-before') {
      steps {
        sh '''#!/bin/bash
# Cidr Block
# Subnet Name

subnet=$(aws ec2 describe-subnets --filters "Name=cidrBlock,Values=$1" "Name=tag:Name,Values=$2" --query "Subnets[0]")

if [ "$subnet" = "null" ]; then
        exit 1
fi

exit 0'''
      }
    }
    stage('Before') {
      steps {
        echo 'non'
      }
    }
  }
}