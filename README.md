## AWS EC2 Auto-Scaling with Load Balancer ##
EC2 Auto-Scaling with Load Balancer using AWS CloudFormation

This project demonstrates how to deploy an EC2 Auto-Scaling Group (ASG) with an Application Load Balancer (ALB) in AWS using a CloudFormation template. The setup ensures high availability, scalability, and fault tolerance.

The template.yaml file contains the complete configuration for:

VPC
Subnets
Internet Gateway
Route Tables
Load Balancer
Auto-Scaling Group with Launch Template


Run the following command to create the CloudFormation stack:

aws cloudformation create-stack --stack-name ec2-asg-lb-stack \
  --template-body file://template.yaml \
  --parameters ParameterKey=KeyName,ParameterValue=your-ssh-key-name

Replace your-ssh-key-name with your actual SSH key pair name.
