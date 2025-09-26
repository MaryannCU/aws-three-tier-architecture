# AWS Three-Tier Architecture Project

## Overview
This project demonstrates how to build a **Three-Tier Application Architecture** on AWS for high availability, scalability, and security.  
It was provisioned directly from the **AWS Management Console**.

## Architecture
- **Web Tier**: Nginx web server running on EC2 in a public subnet  
- **Application Tier**: EC2 instances in a private subnet  
- **Database Tier**: RDS (or placeholder EC2 DB) in a private subnet  
- **Load Balancer**: Application Load Balancer distributing traffic  
- **Networking**: VPC with public and private subnets, Internet Gateway, NAT Gateway  
- **Security**: Security Groups controlling access between tiers  

## Services Used
- **VPC** (custom with subnets)  
- **EC2** (web + app)  
- **RDS or EC2-DB** (database tier)  
- **Elastic Load Balancer**  
- **Target Groups & Health Checks**  
- **Security Groups & NACLs**  

## Steps Followed
1. Created a custom VPC with public and private subnets  
2. Configured Internet Gateway + NAT Gateway  
3. Launched EC2 instances for Web & App tiers  
4. Installed **Nginx** on the Web Tier  
5. Deployed DB in a private subnet  
6. Configured Security Groups (Web → App → DB flow)  
7. Created a Load Balancer and Target Group  
8. Tested deployment by accessing the Load Balancer DNS in browser  


## Screenshots
Screenshots are stored in the [`screenshots/`](screenshots/) folder:
- `nginx-homepage.png`  
- `target-group.png`  
- `load-balancer.png`  
- `vpc-subnets.png`  
- `security-groups.png`  


## Lessons Learned
- Why separating tiers improves reliability & scalability  
- How AWS networking (VPC, subnets, gateways) secures applications  
- Importance of health checks and load balancing  

## Repository
This repo documents my AWS project.  
➡️ Deployed live inside AWS (not using IaC tools).# AWS Three-Tier Architecture Project

