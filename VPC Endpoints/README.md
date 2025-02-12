# **Objective**

The goal of this project is to set up and test VPC endpoints in AWS for secure communication between an EC2 instance and an S3 bucket, without exposing traffic to the public internet.

## **Steps**

1. **Architecture Setup**: Create a VPC with a public subnet, launch an EC2 instance, and set up an S3 bucket.
2. **Connect to EC2 Instance**: Test accessing the S3 bucket via the public internet.
3. **Set Up Access Keys**: Configure access keys to securely interact with AWS resources.
4. **Interact with S3 Bucket**: Test access to the S3 bucket from the EC2 instance using AWS CLI.
5. **Set Up Gateway**: Configure a VPC endpoint for secure communication with S3.
6. **Bucket Policies**: Set up a policy that restricts access to the S3 bucket from only the VPC endpoint.
7. **Update Route Tables**: Update route tables to direct traffic to the VPC endpoint.
8. **Validate Endpoint Connection**: Ensure the EC2 instance can access the S3 bucket securely through the VPC endpoint.

## **Learnings**

- Learned how to set up VPC endpoints for private communication between AWS resources.
- Understood the importance of configuring access keys and IAM roles for secure interactions.
- Gained insight into configuring bucket policies and route tables for restricted access.
- Realized the significance of endpoint policies in controlling traffic between the VPC and AWS services.

