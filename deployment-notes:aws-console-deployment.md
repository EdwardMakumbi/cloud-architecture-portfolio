{\rtf1\ansi\ansicpg1252\cocoartf2867
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica-Bold;\f1\fswiss\fcharset0 Helvetica;\f2\froman\fcharset0 Times-Italic;
\f3\froman\fcharset0 Times-Roman;}
{\colortbl;\red255\green255\blue255;\red0\green0\blue0;}
{\*\expandedcolortbl;;\cssrgb\c0\c0\c0;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\b\fs24 \cf0 AWS Console Deployment Steps \'96 LiveDocApp
\f1\b0 \
\
1. Create a new VPC with public subnets in multiple Availability Zones.\
2. Launch Amazon Linux EC2 instances.\
3. Install Apache web server:\
\
\pard\pardeftab720\partightenfactor0

\f2\i \cf0 \expnd0\expndtw0\kerning0
\outl0\strokewidth0 \strokec2 sudo yum update -y\
sudo yum install httpd -y\
sudo systemctl start httpd\
\

\f3\i0 4. Upload website static files.\
5. Create a Launch Template for Auto Scaling.\
6. Configure Auto Scaling Group with minimum and maximum instances.\
7. Create Classic Load Balancer and attach the ASG.\
8. Create Route 53 hosted zone and point domain to the Load Balancer.\
9. Configure S3 bucket for static content.\
10. Configure CloudFront distribution using the S3 bucket as origin.\
11. Test application access globally and verify health checks.}