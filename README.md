# SPA-Event-Hosting-Infra

This repository manages the infrastructure and CI/CD pipeline for deploying the [SF Events Listing](https://github.com/rohitdalvi18/SPA-Event-Hosting) Single Page Application (SPA) on AWS. It automates nightly builds, smoke tests, and deployment to a QA environment using GitHub Actions, AWS EC2, ECR, RDS, and Nginx.

## 🚀 Features
- Nightly Deployment Workflow (Runs every night at 2 AM UTC)
- Dynamic EC2 for Build & Smoke Tests (Temporary instance for verification)
- Pushes Docker Images to AWS ECR (Backend & Frontend images)
- Deploys Latest Images to a Pre-Allocated QA EC2
- SSL Enabled with Let’s Encrypt & Nginx Reverse Proxy
- Uses GitHub Actions for CI/CD Automation

## 📌 AWS Infrastructure

✅ Pre-Created AWS Resources
- EC2 (QA Instance) → Hosts the final deployed application
- ECR (Container Registry) → Stores backend & frontend images
- RDS (MySQL Database) → Stores event data
- Route 53 (Domain Name) → sf-events.info
- Nginx (Reverse Proxy & SSL) → Handles HTTPS & API requests

##### 🔹 Live App: sf-events.info
##### 🔹 Backend API: sf-events.info/api/
