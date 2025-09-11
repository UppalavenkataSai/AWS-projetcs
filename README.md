# 🚀 AWS Application Load Balancer (ALB) – Hands-On Project

This project demonstrates how to set up a **highly available and fault-tolerant web architecture** using AWS EC2 instances behind an Application Load Balancer (ALB).

---

## 📌 Project Goals

- Set up two EC2 Linux instances in different availability zones
- Install and configure Apache web servers
- Register instances to a target group
- Create and configure an Application Load Balancer
- Secure traffic flow using security groups
- Test load balancing via browser and `curl`

---

## 📁 Architecture Diagram

    Internet (Users)
          ↓
+------------------------------+
| Application Load Balancer |
+--------------+---------------+
↓
┌──────────────┐ ┌──────────────┐
│ EC2 in AZ-1 │ │ EC2 in AZ-2 │
│ Apache Web │ │ Apache Web │
└──────────────┘ └──────────────┘
