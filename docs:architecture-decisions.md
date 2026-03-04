{\rtf1\ansi\ansicpg1252\cocoartf2867
\cocoatextscaling0\cocoaplatform0{\fonttbl\f0\fswiss\fcharset0 Helvetica-Bold;\f1\fswiss\fcharset0 Helvetica;}
{\colortbl;\red255\green255\blue255;}
{\*\expandedcolortbl;;}
\paperw11900\paperh16840\margl1440\margr1440\vieww11520\viewh8400\viewkind0
\pard\tx720\tx1440\tx2160\tx2880\tx3600\tx4320\tx5040\tx5760\tx6480\tx7200\tx7920\tx8640\pardirnatural\partightenfactor0

\f0\b\fs24 \cf0 Architecture Decisions \'96 LiveDocApp
\f1\b0 \
\

\f0\b Compute Layer
\f1\b0 \
- EC2 instances chosen for flexibility and full control\
- Multi-AZ deployment to ensure high availability\
\

\f0\b Load Balancing
\f1\b0 \
- Classic Load Balancer used for simplicity; could upgrade to ALB in future\
\

\f0\b CDN
\f1\b0 \
- CloudFront selected to reduce latency for international users\
- S3 static assets separate from compute to improve performance\
\

\f0\b Traffic Routing
\f1\b0 \
- Route 53 ensures DNS-level global traffic management\
- Health checks ensure users are only routed to healthy instances\
\

\f0\b Security
\f1\b0 \
- Security Groups restrict inbound traffic\
- IAM roles used for S3 and EC2 access}