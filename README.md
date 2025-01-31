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

Create Security Groups to allow only necessary traffic.

2️⃣ Step: Deploy the Presentation Layer (Frontend Web Servers)

Deploy EC2 instances in the public subnet.

Install and configure Apache/Nginx as the web server.

Deploy static frontend files or connect to backend APIs.

Attach an Elastic IP for public accessibility.

3️⃣ Step: Deploy the Application Layer (Backend EC2 Instances)

Launch EC2 instances in private subnets.

Install Node.js/Python/PHP or any backend runtime.

Deploy backend application code to handle business logic.

Use an Auto Scaling Group to handle traffic spikes.

Configure ALB to distribute traffic across backend servers.

4️⃣ Step: Configure Database Layer

Deploy an Amazon RDS (MySQL) instance in private subnets.

Set up Multi-AZ replication for high availability.

Secure the database using Security Groups (only allow access from the application layer).

Configure automated backups and snapshots for disaster recovery.

5️⃣ Step: Testing & Monitoring

Retrieve the ALB URL and test the application.

Check CloudWatch metrics for monitoring CPU, memory, and logs.

Set up AWS CloudTrail to log API requests and security activities.

# 📌 Project Outputs:
After deployment, you’ll have:

✅ A scalable web application accessible via ALB URL.

✅ A private RDS database securely storing application data.

✅ Monitoring & logging enabled for performance tracking.
