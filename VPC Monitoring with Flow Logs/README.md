# **VPC Monitoring with Flow Logs**

## **Objective**
The goal of this project is to set up VPC Flow Logs in AWS for monitoring network activity and troubleshooting connectivity issues between VPCs using peering connections.

## **Steps**

1. **Set Up VPCs**: Create two VPCs (NextWork-1 and NextWork-2) with unique IPv4 CIDR blocks.
2. **Launch EC2 Instances**: Launch EC2 instances in each VPC to test connectivity and monitor network traffic.
3. **Set Up Logs**: Configure VPC Flow Logs to capture network traffic and send the logs to CloudWatch for analysis.
4. **Set IAM Permissions for Logs**: Create IAM policies and roles to enable VPC Flow Logs to write data to CloudWatch.
5. **Ping Testing and Troubleshooting**: Test network connectivity between EC2 instances in different VPCs and troubleshoot any issues.
6. **Set Up a Peering Connection**: Create a peering connection between the VPCs to enable secure communication.
7. **Update VPC Route Tables**: Update route tables to ensure proper traffic flow between VPCs.
8. **Analyze Flow Logs**: Review the captured flow logs to monitor network activity and troubleshoot issues.

## **Learnings**

- Gained hands-on experience in setting up VPC peering and configuring flow logs for monitoring network activity.
- Learned how to troubleshoot connectivity issues using flow logs and route tables.
- Explored AWS IAM policies and roles to securely manage log access.
- Used AWS CloudWatch Logs Insights to query and analyze VPC flow log data for performance optimization.
