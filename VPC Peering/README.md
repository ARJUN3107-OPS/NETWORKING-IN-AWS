# **VPC Peering**

## **Objective**
The goal of this project is to set up a VPC peering connection between two AWS VPCs, allowing secure communication between resources across different VPCs without using the internet.

## **Steps**

1. **Set Up VPCs**: Create two VPCs with unique CIDR blocks (e.g., 10.1.0.0/16 and 10.2.0.0/16) to avoid IP range conflicts.
2. **Create Peering Connection**: Establish a peering connection between the two VPCs, allowing them to communicate securely.
3. **Update Route Tables**: Configure route tables in both VPCs to enable traffic flow between them over the peering connection.
4. **Launch EC2 Instances**: Launch EC2 instances in each VPC to test the peering connection by sending and receiving data.
5. **Use EC2 Instance Connect**: Access EC2 instances using EC2 Instance Connect to verify connectivity.
6. **Test VPC Peering**: Verify the communication between the two instances to ensure the peering connection is working.

## **Troubleshooting**

- **Security Group Configuration**: Initially, my EC2 instance did not allow SSH traffic due to incorrect security group rules. I resolved this by allowing inbound traffic on port 22.
- **Elastic IP Setup**: To resolve connectivity issues, I set up Elastic IPs for static, public IP addresses, ensuring consistent connectivity for testing.
- **Ping Test**: To test the VPC peering, I ran a `ping` command between EC2 instances. A successful ping validated the connection, confirming proper routing and security group settings.

## **Key Concepts**

- **VPC Peering**: A private network link between two VPCs that allows secure communication without internet usage. It enables low-latency, high-security traffic flow by updating route tables and security settings.
- **Elastic IPs**: Static, public IP addresses that allow consistent connectivity to EC2 instances even after restarts or IP changes.
- **Requester vs Accepter**: The **Requester** initiates the peering connection request, while the **Accepter** approves or denies it.

## **Learnings**
- Gained experience in configuring VPC peering, route tables, and security groups.
- Troubleshooted common issues like security group misconfigurations and connectivity errors.
- Used EC2 Instance Connect and Elastic IPs to enhance testability and connectivity.

## **Logs Insights**
Using EC2 Instance Connect and running diagnostic tests like ping helped identify issues quickly, ensuring smooth operation of the peering connection and communication between instances.

