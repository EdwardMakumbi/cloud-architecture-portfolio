### AWS Console Deployment Steps – LiveDocApp

### Step 1. Create a new VPC with public subnets in multiple Availability Zones.
### Step 2. Launch Amazon Linux EC2 instances.

Install Apache web server:
sudo yum update -y, 
sudo yum install httpd -y, 
sudo systemctl start httpd

Upload website static files to EC2.
### Step 3: Auto Scaling Group
1. Create Launch Template.
2. Configure ASG with min/max instance count.
3. Enable health checks and multi-AZ deployment.

### Step 4: Load Balancer
1. Create Classic Load Balancer.
2. Attach ASG to CLB.
3. Configure HTTP listener (Port 80) and health checks.

### Step 5: Static Content Optimization
1. Create S3 bucket for static assets.
2. Upload files.
3. Create CloudFront distribution with S3 as origin.

### Step 6: DNS Configuration
1. Create Route 53 hosted zone.
2. Point A record to Classic Load Balancer.

### Step 7: Testing
1. Access application globally.
2. Verify load balancing and health checks.
