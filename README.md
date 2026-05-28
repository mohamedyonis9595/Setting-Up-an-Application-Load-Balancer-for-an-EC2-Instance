## 📸 Infrastructure Deployment Verification

### 1. Security Infrastructure Topology
Configured a dedicated public-facing Security Group (`devops-sg`) explicitly opening inbound `HTTP` traffic vectors on Port `80` to allow traffic from the open internet:
![AWS ALB Security Group Rules](./images/1.jpg)

### 2. High-Availability Load Balancing Setup
Initiated a Layer 7 Application Load Balancer (`devops-alb`) to balance workloads across the infrastructure:
![AWS ELB Selection](./images/3.jpg)

Configured multi-Availability Zone network mappings to ensure high availability and resilient public routing:
![AWS ALB Network Provisioning](./images/4.jpg)

Linked inbound traffic channels directly to target groups via specialized listener routing mechanics:
![AWS ALB Routing Rules](./images/5.png)

### 3. Backend Target Group Registration
Created the logical target group layer (`devops-tg`) tracking the health status and routing traffic directly to the backend computing assets:
![AWS Target Group Tracking](./images/2.jpg)

Verified security policy attachments directly on the backend compute interfaces to secure communication paths:
![EC2 Interface Configuration](./images/6.png)

### 4. End-to-End Traffic Verification
The live application rendering flawlessly when accessed directly via the globally resolved AWS Application Load Balancer DNS endpoint, confirming complete network and firewall routing alignment:
![Nginx Success Verification](./images/7.png)
