# Architecture Decisions – LiveDocApp

## Compute Layer
- EC2 instances selected for flexibility and full control
- Multi-AZ deployment for high availability

## Load Balancing
- Classic Load Balancer used for simplicity; ALB could be used for path-based routing in future

## CDN & Static Content
- CloudFront selected to reduce latency for global users
- S3 used for static assets to separate compute and storage

## Traffic Routing
- Route 53 ensures global DNS-level traffic management
- Health checks guarantee requests only go to healthy instances

## Security
- Security Groups restrict inbound traffic to HTTP and specific SSH IPs
- IAM roles replace hardcoded credentials
- Network isolation within VPC for safety

## Auto Scaling
- ASG ensures minimum capacity is always available
- Automatically scales based on traffic load

## Monitoring
- CloudWatch monitors EC2 and ASG health
- Provides alerting for system issues
