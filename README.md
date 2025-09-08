# AWS-IAM-Access-Control

A structured **AWS IAM (Identity and Access Management)** setup to efficiently manage users, groups, and permissions in AWS.  
This project demonstrates **role-based access control** 🛡️, security best practices 🔐, and visually documents the architecture with diagrams 📊.

---

## 📚 Table of Contents
- [📖 Overview](#overview)
- [✨ Features](#features)
- [🏗️ IAM Structure](#iam-structure)
- [🗺️ Architecture Diagram](#architecture-diagram)
- [🖼️ Screenshots](#screenshots)
- [🚀 Getting Started](#getting-started)

---

## 📖 Overview
This project focuses on creating a **clear IAM hierarchy** to control access to AWS resources.  
By organizing users into groups and attaching policies at the group level, this setup ensures **scalable and secure permission management**.  
🔒 **Security made simple and scalable!**

---

## ✨ Features
- 🏗️ **Designed an IAM structure** for efficient access control
- 👥 Created **Admins** and **Developers** groups
- 📜 Attached policies:
  - **Admins** → `AmazonS3FullAccess` 🗄️
  - **Developers** → `AmazonEC2FullAccess` ⚡
- 🔄 Users inherit permissions via groups
- 📊 Visualized architecture for clarity and documentation

---

## 🏗️ IAM Structure

### 👫 Groups & Permissions
| 👥 Group       | 🧑‍💻 Users           | 🛡️ Policy Attached         |
|:--------------:|:-------------------:|:-------------------------:|
| **Admins**     | User 1, User 2 | `AmazonS3FullAccess`     |
| **Developers** | Dev1, Dev2          | `AmazonEC2FullAccess`     |

### 🙋‍♂️ Users
- Users are assigned to groups to **inherit permissions automatically**.
- Example: Dev1 and Dev2 belong to Developers Group → EC2 access granted ⚡.

---

## 🗺️ Architecture Diagram

![IAM Architecture Diagram](https://github.com/Naveen15github/AWS-IAM-Access-Control/blob/03053428b6077333d2992edf9a8f820a7a9358ab/IMG_4843.PNG)
> 🖼️ Replace the URL above with your own architecture diagram image hosted in your repo or on an image hosting service.

---

## 🖼️ Screenshots

### 👥 Users
![Admins Group Screenshot](https://github.com/Naveen15github/AWS-IAM-Access-Control/blob/f470ea505e27fd8c979e10a43a5a0adba2d1b6a1/Screenshot%20(15).png)

### 👨‍💻 Groups
![Developers Group Screenshot](https://github.com/Naveen15github/AWS-IAM-Access-Control/blob/f470ea505e27fd8c979e10a43a5a0adba2d1b6a1/Screenshot%20(16).png)

### 📜 Policy Attachment
![Policy Attachment Screenshot](https://github.com/Naveen15github/AWS-IAM-Access-Control/blob/f470ea505e27fd8c979e10a43a5a0adba2d1b6a1/Screenshot%20(14).png)     ![Policy Attachment Screenshot](https://github.com/Naveen15github/AWS-IAM-Access-Control/blob/f470ea505e27fd8c979e10a43a5a0adba2d1b6a1/Screenshot%20(13).png)

---

## 🚀 Getting Started

To replicate this IAM setup:

1. **Login to AWS Management Console** 🔑  
2. Navigate to **IAM → Users / Groups / Policies**  
3. Create groups:  
   - `Admins` 👑  
   - `Developers` 👨‍💻  
4. Attach policies to groups:  
   - Admins → `AmazonS3FullAccess` 🗄️  
   - Developers → `AmazonEC2FullAccess` ⚡  
5. Create users and assign them to appropriate groups 🙋‍♂️  
6. Verify permissions by logging in as a user ✅  

---

## 🔧 Usage

- **Admins**: Access S3 Buckets for storage and management 🗄️  
- **Developers**: Launch and manage EC2 instances ⚡  
- **Scalability**: Add new users to groups without manually assigning individual permissions 📈  

---

## 🛡️ Best Practices

- 🔒 Assign permissions **only at the group level** whenever possible
- ⚖️ Use **least privilege principle** — give users only the access they need
- 🛡️ Enable **MFA** for all users for better security
- 📋 Regularly audit IAM policies and roles

---

✨ **Strengthening the foundations of Cloud Security & Access Management** 🚀

---

#AWS #IAM #CloudComputing #DevOps #AccessControl #LearningInPublic
