# AWS Full stacke Architecture Setup Steps

## 1. Create a VPC

## 2. Create Subnets
- Web Public 1a, 1b
- Web Private 1a, 1b
- App Private 1a, 1b
- DB Private 1a, 1b

## 3. Create Route Tables
- Web Public
- Web Private 1a, 1b
- App Private 1a, 1b
- DB Private 1a, 1b

## 4. Associate Route Tables with Subnets

## 5. Create Internet Gateway (IGW) and Attach to VPC

## 6. Create NAT Gateway (NATGW) in Web Public Subnet

## 7. Add Routes to Route Tables
- Public → IGW
- Private → NATGW

## 8. Create Security Groups
- Frontend ALB
- Frontend Servers
- Backend ALB
- Backend Servers
- DB Private Servers

## 9. Create Database Subnet Group

## 10. Create Database Server

## 11. Create Frontend ALB
- Create Frontend ALB Target Group

## 12. Create Backend ALB
- Create Backend ALB Target Group

## 13. Create Frontend Server AMI
- Install Nginx
- Install Git

## 14. Create Backend Server AMI
- Install PHP, MySQL, Apache
- Install Git
- Run the database script

## 15. Create Launch Template for Frontend Server

## 16. Create Launch Template for Backend Server

## 17. Create Auto Scaling Group for Frontend Server

## 18. Create Auto Scaling Group for Backend Server