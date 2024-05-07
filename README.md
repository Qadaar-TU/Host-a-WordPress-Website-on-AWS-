# Hosting a WordPress Website on AWS

This project aims to deploy a WordPress website on AWS utilizing various resources and best practices in cloud architecture and DevOps methodologies. Below is a summary of the configuration and deployment process:

## Overview

The project involves configuring a Virtual Private Cloud (VPC) with both public and private subnets across multiple availability zones. It leverages various AWS services such as EC2, NAT Gateway, Application Load Balancer, Route 53, RDS, EFS, Certificate Manager, and Simple Notification Service (SNS) to create a scalable, fault-tolerant, and secure WordPress hosting environment.

## Project Steps

1. **VPC Configuration**: Created a VPC with public and private subnets across multiple availability zones to enhance fault tolerance and reliability.

2. **Internet Gateway**: Deployed an Internet Gateway to facilitate connectivity between VPC instances and the wider Internet.

3. **Security Groups**: Established Security Groups as a network firewall mechanism to control inbound and outbound traffic to EC2 instances.

4. **Availability Zones**: Leveraged two Availability Zones to enhance system reliability and fault tolerance.

5. **Public Subnets**: Utilized Public Subnets for infrastructure components like the NAT Gateway and Application Load Balancer.

6. **EC2 Instance Connect Endpoint**: Implemented EC2 Instance Connect Endpoint for secure connections to assets within both public and private subnets.

7. **Private Subnets**: Positioned web servers (EC2 instances) within Private Subnets for enhanced security.

8. **NAT Gateway**: Enabled instances in both the private Application and Data subnets to access the Internet via the NAT Gateway.

9. **WordPress Deployment**: Hosted the website on EC2 Instances.

10. **Application Load Balancer**: Employed an Application Load Balancer and a target group for evenly distributing web traffic to an Auto Scaling Group of EC2 instances across multiple Availability Zones.

11. **Auto Scaling Group**: Utilized an Auto Scaling Group to automatically manage EC2 instances, ensuring website availability, scalability, fault tolerance, and elasticity.

12. **Version Control**: Stored web files on GitHub for version control and collaboration.

13. **Certificate Manager**: Secured application communications using a Certificate Manager.

14. **Simple Notification Service (SNS)**: Configured SNS to alert about activities within the Auto Scaling Group.

15. **Route 53**: Registered the domain name and set up a DNS record using Route 53.

16. **EFS**: Used EFS for shared file system.

17. **RDS**: Utilized RDS for the database.

## Repository

The reference diagram and deployment scripts used for this project are uploaded to a GitHub repository. You can access the repository [here]([repository_url](https://github.com/Qadaar-TU/Host-a-WordPress-Website-on-AWS-/tree/main)).

Feel free to explore the repository for more details on the project configuration and deployment process.

[Repository URL]([repository_url](https://github.com/Qadaar-TU/Host-a-WordPress-Website-on-AWS-/tree/main))

## Conclusion

By following the steps outlined above and utilizing AWS services effectively, we have successfully deployed a scalable, fault-tolerant, and secure WordPress website on AWS. This project demonstrates best practices in cloud architecture and DevOps methodologies for hosting web applications on AWS infrastructure.
