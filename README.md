# AWS-Three-Tier-Architecture-Project
# 📌 Project Overview:
This project demonstrates the deployment of a scalable, secure, and highly available 3-tier web application on AWS. The 3-tier architecture separates the application into three layers:

1️⃣ Presentation Layer – Handles user requests (Frontend Web Servers)
2️⃣ Application Layer – Processes business logic (Backend EC2 Instances)
3️⃣ Data Layer – Manages storage & databases (Amazon RDS)

This architecture is commonly used by real-world applications such as e-commerce platforms, enterprise applications, and SaaS solutions.

# 📸 Architecture Diagram:
![3-Tier Architecture](https://github.com/user-attachments/assets/450f1f1d-7413-41d8-a59a-7964e9847322)

# 🚀 Project Setup & Deployment:
1️⃣ Step: Create the Network

Set up a VPC with public & private subnets.

Configure Internet Gateway & NAT Gateway for connectivity.

2️⃣ Step: Deploy the Application Layer

Launch EC2 instances in private subnets.

Use an Auto Scaling Group to handle traffic spikes.

Set up an Application Load Balancer in public subnets.

3️⃣ Step: Configure Database Layer

Deploy an Amazon RDS (MySQL) instance in private subnets.

Secure it using security groups (only allow access from the application layer).

4️⃣ Step: Testing & Monitoring

Retrieve the ALB URL and test the application.

Monitor logs & performance using CloudWatch.

# 📌 Project Outputs:
After deployment, you’ll have:
✅ A scalable web application accessible via ALB URL.
✅ A private RDS database securely storing application data.
✅ Monitoring & logging enabled for performance tracking.
