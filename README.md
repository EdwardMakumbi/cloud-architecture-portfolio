{\rtf1\ansi\ansicpg1252\cocoartf2867
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica-Bold;\f1\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\b\fs24 \cf0 LiveDocApp \'96 Highly Available Online Doctor\'92s Clinic Deployment (AWS)
\f1\b0 \
\

\f0\b Project Overview\

\f1\b0 \
LiveDocApp is a cloud-based web application designed to provide reliable and scalable online doctor\'96patient interactions.  \
The goal was to deploy the application on AWS with high availability, global accessibility, performance optimisation, and fault tolerance using core cloud architecture principles.\
\

\f0\b \
Architecture design
\f1\b0 \
The architecture ensures:\
\
- High availability across multiple EC2 instances\
- Traffic distribution using Classic Load Balancer\
- Global content acceleration via CloudFront CDN\
- DNS-based traffic routing with Route 53\
- Auto Scaling to handle variable load\
- Separation of static and compute layers\
\

\f0\b Technologies Used
\f1\b0 \
\
- Amazon EC2 (Linux)\
- Auto Scaling Group (ASG)\
- Classic Load Balancer (CLB)\
- Amazon S3\
- Amazon CloudFront\
- Amazon Route 53\
- Apache Web Server\
- HTML / CSS / JavaScript\
- IAM Roles & Security Groups\
\

\f0\b Scalability & High Availability\

\f1\b0 \
- Multi-instance deployment prevents downtime\
- Auto Scaling dynamically adjusts capacity\
- Load Balancer eliminates single point of failure\
- Deployment across multiple Availability Zones increases fault tolerance\
- CloudFront reduces load on origin infrastructure\
\

\f0\b Security Considerations\

\f1\b0 \
- Security Groups allow HTTP (Port 80) only\
- SSH restricted to specific IP addresses\
- IAM roles used instead of hardcoded credentials\
- Instances isolated within VPC\
\

\f0\b Cost Optimisation
\f1\b0 \
\
- Auto Scaling prevents over-provisioning\
- Instances scale based on demand\
- CloudFront + S3 reduces compute overhead\
- Pay-as-you-go model\
\

\f0\b Result / Impact\

\f1\b0 \
- High availability for online doctor-patient interactions\
- Global performance improvements through CloudFront CDN\
- Fault-tolerant, production-ready cloud infrastructure\
- Demonstrated practical AWS architecture implementation skills\
\

\f0\b Skills Demonstrated
\f1\b0 \
\
- AWS Infrastructure Design\
- High Availability Architecture\
- Auto Scaling Configuration\
- Load Balancer Setup\
- DNS & Traffic Engineering\
- CDN Optimisation\
- Secure Cloud Deployment\
- Cloud Performance Optimisation\
\

\f0\b Future Improvements
\f1\b0 \
\
- Migrate from Classic Load Balancer to Application Load Balancer\
- Implement HTTPS with ACM certificates\
- Add Web Application Firewall (WAF)\
- Convert deployment to Infrastructure as Code (Terraform)\
- Integrate CI/CD pipeline via GitHub Actions\
}