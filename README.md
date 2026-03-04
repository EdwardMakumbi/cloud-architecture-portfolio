## LiveDocApp : Highly Available Online Doctor's Clinic Deployment (AWS)

## Project Overview

## LiveDocApp is a cloud-based web application designed to provide reliable and scalable online doctor–patient interactions.  
The goal was to deploy the application on AWS with high availability, global accessibility, performance optimization, and fault tolerance using core cloud architecture principles.

## Architecture Summary
The architecture ensures:

- High availability across multiple EC2 instances
- Traffic distribution using Classic Load Balancer
- Global content acceleration via CloudFront CDN
- DNS-based traffic routing with Route 53
- Auto Scaling to handle variable load
- Separation of static and compute layers

## Technologies Used

- Amazon EC2 (Linux)
- Auto Scaling Group (ASG)
- Classic Load Balancer (CLB)
- Amazon S3
- Amazon CloudFront
- Amazon Route 53
- Apache Web Server
- HTML / CSS / JavaScript
- IAM Roles & Security Groups

## Scalability & High Availability
- Multi-instance deployment prevents downtime
- Auto Scaling dynamically adjusts capacity
- Load Balancer eliminates single point of failure
- Deployment across multiple Availability Zones increases fault tolerance
- CloudFront reduces load on origin infrastructure

## Security Considerations
- Security Groups allow HTTP (Port 80) only
- SSH restricted to specific IP addresses
- IAM roles used instead of hardcoded credentials
- Instances isolated within VPC

## Cost Optimization
- Auto Scaling prevents over-provisioning
- Instances scale based on demand
- CloudFront + S3 reduces compute overhead
- Pay-as-you-go model

## Result / Impact
- High availability for online doctor-patient interactions
- Global performance improvements through CloudFront CDN
- Fault-tolerant, production-ready cloud infrastructure
- Demonstrated practical AWS architecture implementation skills

## Skills Demonstrated

- AWS Infrastructure Design
- High Availability Architecture
- Auto Scaling Configuration
- Load Balancer Setup
- DNS & Traffic Engineering
- CDN Optimization
- Secure Cloud Deployment
- Cloud Performance Optimization


## Future Improvements
- Migrate from Classic Load Balancer to Application Load Balancer
- Implement HTTPS with ACM certificates
- Add Web Application Firewall (WAF)
- Convert deployment to Infrastructure as Code (Terraform)
- Integrate CI/CD pipeline via GitHub Actions
