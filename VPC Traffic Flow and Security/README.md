# **VPC Traffic Flow and Security**

## **Objective**
This project focuses on setting up and securing network traffic flow in an Amazon VPC by using route tables, security groups, and network ACLs. It ensures secure communication within isolated subnets and with the internet.

## **Steps**

1. **Set Up Route Tables**: I created route tables that define how traffic is directed across subnets and to the internet. For public subnets, the route table sends outbound traffic to an Internet Gateway (IGW).
2. **Configure Security Groups**: I configured security groups as virtual firewalls to control inbound and outbound traffic for EC2 instances, specifying rules for HTTP (port 80) and SSH (port 22).
3. **Use Network ACLs**: Network ACLs were applied to control inbound and outbound traffic at the subnet level, adding an additional layer of security beyond security groups.
4. **Adjust Rules for Traffic Flow**: I adjusted both security groups and network ACLs to ensure secure communication and traffic flow between the subnets and the internet.

## **Key Concepts**

- **Route Tables**: These determine how traffic is routed within a VPC. For public subnets, traffic is directed through an Internet Gateway (IGW).
- **Security Groups**: Stateful firewalls that control traffic at the instance level. Rules define allowed inbound and outbound traffic.
  - **Inbound Rules**: Control traffic entering an instance (e.g., HTTP on port 80, SSH on port 22).
  - **Outbound Rules**: Control traffic leaving an instance (by default, all outbound traffic is allowed).
- **Network ACLs**: Stateless firewalls that control traffic at the subnet level. Unlike security groups, ACLs are more restrictive and require explicit allow rules for communication.

## **Default vs. Custom Network ACLs**

- **Default Network ACLs**: Allow all inbound and outbound traffic by default, which can be modified for more granular control.
- **Custom Network ACLs**: Start with deny-all inbound and outbound rules, and you must create allow rules to define permissible traffic, making them more restrictive.

## **Challenges and Learnings**
- I didn’t expect the need to adjust both security groups and network ACLs simultaneously for a seamless traffic flow. This granular control required more configuration than initially anticipated.

## **Project Time**
This project took me approximately **1 hour** to complete, involving setting up route tables, configuring security groups and network ACLs, and testing traffic flow.

## **Conclusion**
By implementing VPC traffic flow and security measures using route tables, security groups, and network ACLs, I was able to establish a secure network environment that allows efficient and controlled communication within the VPC and to the internet.
