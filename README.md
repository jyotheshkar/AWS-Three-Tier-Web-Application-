# Three-Tier Web Application using AWS

This project demonstrates the creation of a secure, scalable three-tier architecture using Amazon Web Services. The application allows users to retrieve data in real-time from a DynamoDB database through a static website hosted on S3 and distributed globally via CloudFront.

## 🛠️ AWS Services Used
- **Amazon S3** – for hosting static web files (HTML, CSS, JavaScript)
- **Amazon CloudFront** – for content delivery and global distribution
- **AWS Lambda** – for serverless compute to process API logic
- **Amazon API Gateway** – for creating and managing RESTful APIs
- **Amazon DynamoDB** – for NoSQL database and data storage

## 📁 Architecture Overview
- **Presentation Tier**: Built with Amazon S3 and delivered via CloudFront using Origin Access Control (OAC) to enhance security.
- **Logic Tier**: Implemented using AWS Lambda functions and API Gateway, enabling serverless data retrieval.
- **Data Tier**: DynamoDB table with `userId` as partition key to store and retrieve user-related information.

## ✅ Key Features
- Real-time data retrieval from the database via user interactions
- Secure Lambda permissions using custom inline IAM policies
- CORS configuration and header management for cross-origin requests
- Error handling, response structuring, and full API documentation
- Performance-tested content delivery with CloudFront vs S3

## 🔗 Documentation
This repository includes four detailed PDF documents explaining each part of the architecture:
1. **CloudFront Presentation Tier**
2. **API Gateway + Lambda Logic Tier**
3. **DynamoDB Data Tier + Lambda Integration**
4. **Three-Tier Architecture Integration & Troubleshooting**

## 📸 Demo Screenshots (Optional)
You can add screenshots here showing:
- S3 bucket file structure
- API Gateway configuration
- CloudFront distribution settings
- JSON Lambda test output

## 📂 Project Status
✅ Completed  
📅 March 2025  
📍 Personal Learning Project – Part of AWS Architecture Practice

## 🔗 Live Preview / Deployment
*Link to CloudFront Distribution (if applicable)*  
*Link to GitHub-hosted PDFs (see /docs folder)*

---
Made by [Jyothesh Karnam](https://github.com/jyotheshkar)
