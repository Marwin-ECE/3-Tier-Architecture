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

## Objectives
This project aims to:

1. **Design and implement a highly available 3-tier architecture** on AWS.
2. **Deploy web, application, and database tiers** across multiple Availability Zones.
3. **Secure the infrastructure** using Security Groups.
4. **Demonstrate practical AWS skills**, including VPC setup, EC2 deployment, RDS configuration, and networking.
5. **Verify connectivity and functionality** between all tiers of the architecture.


---

## Step 1: VPC Setup
- Created a VPC
- 4 subnets (1 public, 3 private)
- Enabled public IP addresses for public subnet
- Allocated Elastic IP
- Created Internet Gateway and NAT Gateway
- Configured Route Tables for public and private subnets

## Creating VPC, Subnets, Route tables, Internet and NAT Gateway
<img width="2879" height="1469" alt="Image" src="https://github.com/user-attachments/assets/1708faca-b05e-4a31-96b3-4a552333b533" />

<img width="2879" height="1464" alt="Image" src="https://github.com/user-attachments/assets/4026ae91-69a1-482b-bf5d-5018cabeb7c4" />

<img width="2879" height="1466" alt="Image" src="https://github.com/user-attachments/assets/31131483-5119-4bbe-9849-1a1aff975f28" />

<img width="2879" height="1461" alt="Image" src="https://github.com/user-attachments/assets/5475ce1d-389a-4116-b568-b703a72f566c" />

<img width="2878" height="1461" alt="Image" src="https://github.com/user-attachments/assets/f37a7365-2ad9-4d36-b8e5-e7fe97159c92" />

## Step 2: Configuring Security Groups
- Created Security Groups for Bastion Host, Web Server, App Server, Database
- Linked Security Groups with each other
- Configured inbound rules for each Security Group

## Security Groups
<img width="2873" height="1458" alt="Image" src="https://github.com/user-attachments/assets/2e191407-cf54-444a-9b1a-6348d0835399" />

## Step 3: Creating Bastion Host
- EC2 instance in **public subnet**
- Applied Bastion Host Security Group

<img width="2879" height="1455" alt="Image" src="https://github.com/user-attachments/assets/b3e072f0-e82e-475f-8ac4-561a3f537480" />

## Step 4: Web Server
- EC2 instance in **public subnet**
- Applied Web Server Security Group

<img width="2867" height="1453" alt="Image" src="https://github.com/user-attachments/assets/75eaf255-39a3-47dc-a602-f85af7ae2061" />

## Step 5: App Server
- EC2 instance in **private subnet**
- Applied App Server Security Group
<img width="2877" height="1461" alt="Image" src="https://github.com/user-attachments/assets/695fdc53-9bc6-4fb2-a725-9b32ec51d386" />

## Step 6: Database Server (RDS)
- Created **RDS subnet group**
- Deployed **MariaDB instance** (Free Tier)
- Disabled automated backups & encryption

<img width="2868" height="1457" alt="Image" src="https://github.com/user-attachments/assets/e78df5de-c27a-4118-a484-9d00ff6a3550" />

## Step 7: SSH & Connectivity Tests
- Uploaded SSH keys to Bastion Host
- Connected to App Server via Bastion
- Tested ping to Web Server and MySQL connection to DB

<img width="2011" height="132" alt="Image" src="https://github.com/user-attachments/assets/1fcefae8-ff72-42bc-9e1b-ff95abe1cbbb" />

<img width="2878" height="1700" alt="Image" src="https://github.com/user-attachments/assets/50ef8fd1-1480-4582-b790-2cb91f4b16b9" />

<img width="2879" height="1706" alt="Image" src="https://github.com/user-attachments/assets/5c81cbbe-7693-404e-bf1e-82ae8cfed271" />

## Skills Demonstrated
- AWS Cloud Architecture & Networking
- High Availability Setup
- Linux CLI & Bash scripting
- EC2 & RDS deployment
- Security Groups & Secure SSH Access

---

## Notes
All implementations and screenshots are my own work based on **AWS re/Start hands-on labs**.





