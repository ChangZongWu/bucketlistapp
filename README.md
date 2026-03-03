# 🪣 Bucket List Tracker (AWS Full-Stack Application)

Live Demo:  
👉 https://main.d2w72mfbxoh3jx.amplifyapp.com/

---

## 📌 Overview

Bucket List Tracker is a full-stack cloud application built with React and AWS Amplify.

Users can:

- 🔐 Sign up and log in securely
- ➕ Create bucket list items
- 📝 Add descriptions
- 🖼 Upload images
- ❌ Delete items
- 🔒 Access only their own data

This project demonstrates real-world serverless cloud architecture using AWS managed services.

---

## 🏗 Architecture

![Architecture Diagram](assets/bucketList.png)

---

## 🚀 Tech Stack

### Frontend
- React (Vite)
- AWS Amplify UI Components
- JavaScript (ES6+)

### Backend (AWS Cloud)
- AWS Amplify Hosting
- AWS Cognito (Authentication)
- AWS AppSync (GraphQL API)
- Amazon DynamoDB (Database)
- Amazon S3 (Image Storage)

---

## 🔄 How It Works

1. User accesses the deployed Amplify web application.
2. Authentication is handled by AWS Cognito.
3. React frontend communicates with AWS AppSync (GraphQL API).
4. AppSync performs CRUD operations on DynamoDB.
5. Uploaded images are securely stored in Amazon S3.
6. Owner-based authorization ensures users only see their own data.

---

## 🔐 Authentication & Authorization

- Managed by AWS Cognito
- Email-based login system
- Owner-based access control using userPools
- Secure identity-based S3 storage paths

---

## 🗄 Data Model

BucketItem Model:

id: ID  
title: String  
description: String  
image: String  
createdAt: AWSDateTime  
updatedAt: AWSDateTime  

Each record is protected with owner-based authorization rules.

---

## 📦 Features

✔ Secure user authentication  
✔ GraphQL API integration  
✔ Real-time CRUD operations  
✔ Image upload to Amazon S3  
✔ Owner-based data protection  
✔ Cloud deployment with CI/CD  

---

## 🛠 Local Development

### 1️⃣ Clone Repository

git clone <your-repo-url>  
cd bucketlistapp  

### 2️⃣ Install Dependencies

npm install  

### 3️⃣ Run Locally

npm run dev  

---

## ☁ Deployment

This application is deployed using AWS Amplify Hosting.

On every:

git push origin main  

Amplify automatically:
- Builds the application
- Deploys it
- Updates the production URL

---

## 📚 What This Project Demonstrates

- Full-stack cloud development
- Authentication & authorization
- GraphQL API design
- Serverless architecture
- Secure file storage
- CI/CD deployment pipeline

---

## 👨‍💻 Developer

Jerry Wu  
Computer Science Student (Graduating May 2026)  
Interested in Backend & Cloud Engineering  

---
