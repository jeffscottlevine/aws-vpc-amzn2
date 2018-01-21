# aws-cf-vpc-amazon-linux-2
AWS CloudFormation template that creates an Amazon VPC and EC2 instance running Amazon Linux 2

This AWS Cloudformation template does the following:

1. Creates an Amazon Linux 2 VPC with an Internet gateway, routing table, public subnet and so forth.
2. Defines a custom AWS Lambda-backed resource that looks up the AMI based on a name filter.
3. Defines a Lambda function for the aforementioned resource. 
4. Creates an Amazon EC2 instance using the Amazon Linux 2 AMI.

Notes:

1. If you're looking for an example of a name filter, here's an example: amzn2-ami-hvm*ebs
