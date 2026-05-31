# AWS VPC Architecture — Project Notes

## Network Design
- VPC CIDR: 10.0.0.0/16
- Public Subnet: 10.0.1.0/24
- Private Subnet: 10.0.2.0/24

## Components Used
- Internet Gateway — public internet access
- NAT Gateway — private subnet outbound traffic
- Security Groups — port 80, 443 inbound allowed
- Network ACLs — subnet level firewall
- Route Tables — separate for public and private
- CloudWatch — network monitoring and alerts

## Security Rules
- Public subnet: HTTP/HTTPS traffic only
- Private subnet: accessible only from public subnet
- No direct internet access to private subnet

## Skills Demonstrated
- Subnetting and CIDR notation
- Cloud network segmentation
- AWS firewall configuration
- Network security best practices
