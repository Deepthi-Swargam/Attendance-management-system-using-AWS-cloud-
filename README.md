# Attendance Management System using AWS Cloud ☁️

This project presents a **cloud-based attendance tracking system** designed to manage student attendance efficiently using Amazon Web Services (AWS). It replaces manual attendance with a digital, scalable solution that can be deployed and accessed from anywhere.

## 🧩 Abstract

The system allows authorized users to:
- Add and manage student records
- Mark daily attendance
- Generate reports
- Store data securely on the cloud

This system improves **accuracy**, **accessibility**, and **reduces human error**, especially in large institutions.

## 🔧 Technologies Used

- **Backend:** Python (optional: Flask/Lambda)
- **Database:** AWS RDS (MySQL)
- **Cloud Services:**
  - AWS RDS – for storing attendance records
  - AWS S3 – for optional file storage
  - AWS Lambda – to handle backend logic
  - AWS API Gateway – for routing API requests
  - AWS IAM – to manage access and roles
  - AWS CloudWatch – for logging and monitoring

## 📁 Modules

- **Admin Module**: Can add/remove students and manage attendance
- **Student Module**: Can view attendance status (optional)
- **Database Module**: Stores student info and attendance logs

## ⚙️ How It Works

1. Admin logs in and selects a class
2. System fetches student list from AWS RDS
3. Attendance is marked and stored in the database
4. Reports can be generated for any date range
5. Entire system is deployed on AWS for reliability and scalability

## 📊 Database Schema

**Student Table**
- `student_id` (Primary Key)
- `name`
- `roll_no`
- `branch`
- `year`

**Attendance Table**
- `attendance_id` (Primary Key)
- `student_id` (Foreign Key)
- `date`
- `status` (Present/Absent)

## ✅ Features

- Real-time data storage on AWS
- Secure and role-based access
- Clean UI (optional frontend)
- Scalability using cloud infrastructure

## 🔐 Security

- IAM roles control access to AWS resources
- CloudWatch logs all activity
- Optional MFA for admin login

## 🚀 Future Scope

- Integration with biometric or facial recognition (using AWS Rekognition)
- SMS/email alerts for attendance
- Analytics dashboard with graphs

## 👨‍💻 Developed by

Deepthi  
Internship at Intrainz 
