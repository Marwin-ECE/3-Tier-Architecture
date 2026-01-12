# AWS 3-Tier Architecture Project

## Project Overview
This project demonstrates the design and implementation of a **highly available 3-tier architecture** on AWS.  
The architecture includes a **web tier**, **application tier**, and **database tier** deployed across multiple Availability Zones. 

## Services Used
- Amazon VPC
- Subnets (Public & Private)
- Internet Gateway, NAT Gateway, Elastic IP
- EC2 (Bastion Host, Web Server, App Server)
- Security Groups
- Amazon RDS (MariaDB)

---

## Step 1: VPC Setup
- Created a VPC
- 4 subnets (1 public, 3 private)
- Enabled public IP addresses for public subnet
- Allocated Elastic IP
- Created Internet Gateway and NAT Gateway
- Configured Route Tables for public and private subnets

<img width="2879" height="1469" alt="Image" src="https://github.com/user-attachments/assets/1708faca-b05e-4a31-96b3-4a552333b533" />


