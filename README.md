# Optimizing Web Application Performance with AWS Load Balancing & Auto Scaling

## 📌 Project Overview
This project focuses on optimizing the performance and scalability of a **simple E-Commerce website** using AWS services like **Elastic Load Balancer (ELB), Auto Scaling, and S3**. By implementing these cloud solutions, the application achieves improved uptime, better resource utilization, and reduced latency.

## 🛠 Tech Stack & Services Used
- **Frontend:** HTML, CSS (Static Web Pages)
- **Backend:** Not included (can be expanded with Node.js, Python, or Java)
- **AWS Services:**
  - **Elastic Load Balancer (ELB)** – Distributes traffic across multiple instances
  - **Auto Scaling Groups** – Dynamically adjusts resources based on demand
  - **Amazon S3** – Stores static assets like images, CSS, and JavaScript files
  - **AWS CloudWatch** – Monitors performance and scaling metrics

## 🚀 Features & Benefits
- **High Availability:** ELB ensures that traffic is evenly distributed, preventing server overload.
- **Scalability:** Auto Scaling adjusts instances dynamically based on user demand.
- **Improved Load Time:** Static assets are stored in **Amazon S3**, reducing server load and improving response time.
- **Monitoring & Alerts:** AWS CloudWatch provides insights into traffic patterns and system health.

## 🏗 Architecture Diagram
```
User → ELB → Auto Scaling Group → EC2 Instances → S3 (Static Files)
```

## ⚙️ Setup & Deployment
### **Step 1: Setup an S3 Bucket**
1. Go to the **AWS S3 Console**.
2. Create a new **S3 bucket** and enable public access.
3. Upload your **HTML, CSS, and JS files**.
4. Enable **static website hosting**.

### **Step 2: Configure an Elastic Load Balancer (ELB)**
1. Go to the **AWS EC2 Console** → Load Balancers.
2. Click on **Create Load Balancer**.
3. Choose **Application Load Balancer (ALB)**.
4. Set up a **target group** and add EC2 instances.

### **Step 3: Configure Auto Scaling**
1. Create a **Launch Template** with EC2 instance details.
2. Set up an **Auto Scaling Group** to manage instances.
3. Define scaling policies (e.g., scale up when CPU > 70%).

### **Step 4: Monitor & Optimize with CloudWatch**
1. Set up **CloudWatch Alarms** for CPU utilization and response times.
2. Enable **logs & monitoring dashboards**.

## 📊 Results (Before & After Optimization)
| Metric          | Before Optimization | After Optimization |
|---------------|-------------------|----------------|
| Uptime        | ~90%              | 92.9%          |
| Load Time     | ~3s               | ~1.2s          |
| Auto Scaling  | No                 | Enabled        |
| Cost Savings  | High fixed costs   | Optimized usage |

## 🔥 Future Improvements
- **Implement a Backend** using Node.js or Python for dynamic content.
- **Use AWS RDS** for database management.
- **Enable CloudFront CDN** for faster global content delivery.

## 🤝 Contributions
Feel free to fork this repository and contribute! Suggestions and improvements are welcome. 🚀


