# 🌐 Cloud Network VPC Architecture Project

## 📌 Project Overview
Designed and implemented a multi-tier AWS VPC (Virtual Private Cloud) architecture simulating a real-world enterprise network environment. This project demonstrates hands-on cloud networking skills including subnetting, security configuration, and network segmentation.

## 🎯 Objective
To design a secure, scalable cloud network on AWS that separates public and private resources using industry-standard networking practices.

## 🏗️ Architecture Design

### Network Components:
- **VPC** — Custom Virtual Private Cloud (CIDR: 10.0.0.0/16)
- **Public Subnet** — For web servers / load balancers (10.0.1.0/24)
- **Private Subnet** — For databases / backend servers (10.0.2.0/24)
- **Internet Gateway** — Allows public subnet internet access
- **NAT Gateway** — Allows private subnet outbound internet access
- **Route Tables** — Separate routing for public and private subnets
- **Security Groups** — Firewall rules for inbound/outbound traffic
- **Network ACLs** — Additional subnet-level security layer

## 🔧 AWS Services Used
| Service | Purpose |
|---|---|
| Amazon VPC | Virtual network creation |
| EC2 | Virtual servers in subnets |
| Internet Gateway | Public internet access |
| NAT Gateway | Private subnet outbound access |
| Security Groups | Instance-level firewall |
| Network ACL | Subnet-level firewall |
| Route Tables | Traffic routing rules |
| CloudWatch | Network monitoring |

## 🛡️ Security Implementation
- Public subnet — only HTTP (80) and HTTPS (443) traffic allowed
- Private subnet — only accessible from public subnet, not from internet
- All outbound traffic from private subnet routed through NAT Gateway
- Network ACLs configured as second layer of defence

## 📚 Key Concepts Demonstrated
- ✅ Subnetting and CIDR notation
- ✅ Public vs Private network segmentation
- ✅ Cloud firewall configuration (Security Groups + NACLs)
- ✅ Internet Gateway vs NAT Gateway difference
- ✅ Route table configuration
- ✅ AWS Free Tier hands-on experience

## 🔗 Related Skills
TCP/IP | DNS | DHCP | AWS Networking | Network Security | Cloud Infrastructure

## 👩‍💻 Author
**Riya Yadav** — Cloud Network Engineer (Fresher)
[LinkedIn](https://www.linkedin.com/in/riya-yadav-1059ba256)
