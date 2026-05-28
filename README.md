### 1. Security Infrastructure Topology

Configured a dedicated public-facing Security Group (devops-sg) explicitly opening inbound HTTP traffic vectors on Port 80 to allow traffic from the open internet:

![Image 1](./images/1.jpg)

### 2. High-Availability Load Balancing Setup

Initiated a Layer 7 Application Load Balancer (devops-alb) to balance workloads across the infrastructure:

![Image 3](./images/3.jpg)

Configured multi-Availability Zone network mappings to ensure high availability and resilient public routing:

![Image 4](./images/4.jpg)

Linked inbound traffic channels directly to target groups via specialized listener routing mechanics:

![Image 5](./images/5.png)

### 3. Backend Target Group Registration

Created the logical target group layer (devops-tg) tracking the health status and routing traffic directly to the backend computing assets:

![Image 2](./images/2.jpg)

Verified security policy attachments directly on the backend compute interfaces to secure communication paths:

![Image 6](./images/6.png)

### 4. End-to-End Traffic Verification

The live application rendering flawlessly when accessed directly via the globally resolved AWS Application Load Balancer DNS endpoint, confirming complete network and firewall routing alignment:

![Image 7](./images/7.png)
