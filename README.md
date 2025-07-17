# 🚀 Masai Library - PDF Resource Platform

[![AWS Static Hosting](https://img.shields.io/badge/AWS-Static%20Hosting-orange?logo=amazon-aws)](https://aws.amazon.com/s3/)
[![Infrastructure as Code](https://img.shields.io/badge/IaC-CloudFormation%20%2B%20Terraform-blueviolet)](https://aws.amazon.com/cloudformation/)
[![Analytics](https://img.shields.io/badge/Analytics-Google%20Analytics-brightgreen)](https://analytics.google.com)
[![Uptime](https://img.shields.io/badge/Uptime-100%25-brightgreen)](https://masailibrary.com)
[![Growth](https://img.shields.io/badge/Growth-152%25%20MoM-success)](https://masailibrary.com)

> A high-performance PDF resource platform serving **900+ monthly active users** with specialized technical content

## 🌟 Key Highlights

- **Scalable Architecture**: Serverless AWS infrastructure handling 5K+ monthly PDF downloads
- **Explosive Growth**: 152% month-over-month traffic increase (2.7K → 6.8K views)
- **Global Reach**: Users from 7+ countries with strong India presence (811 active users)
- **Optimized Performance**: 98/100 Google Lighthouse score with 500ms load times
- **Automated Analytics**: CI/CD pipeline for performance tracking and reporting

## 📊 Performance Snapshot (Last 28 Days)

| Metric | Value | Growth |
|--------|-------|--------|
| **Active Users** | 897 | ↑101.1% |
| **New Users** | 896 | ↑175.6% |
| **PDF Downloads** | 5.9K | ↑1253.7% |
| **Avg Session** | 1m 50s | - |
| **Bounce Rate** | 42.4% | - |

![User Growth Timeline](screenshots/engagement/user_growth_timeline.png)

## 🧩 Technical Architecture

```mermaid
graph LR
    A[User] --> B[CloudFront CDN]
    B --> C[S3 Bucket<br><em>Static Hosting</em>]
    C --> D[Lambda@Edge<br><em>URL Rewrites</em>]
    B --> E[WAF<br><em>Security Rules</em>]
    C --> F[Google Analytics<br><em>Event Tracking</em>]
    G[CI/CD Pipeline] --> C
    H[Terraform] --> I[CloudFormation]
