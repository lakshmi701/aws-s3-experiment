# Secure Cloud Storage Management using AWS S3 Buckets

## 📌 Experiment Title

Secure Cloud Storage Management using AWS S3 Buckets using AWS CLI

---

## 🎯 Objective

To install AWS CLI, configure it, and perform creation and deletion of S3 buckets using AWS CLI.

---

## 🛠️ Tools Used

* AWS CLI
* Amazon S3
* IAM (Identity and Access Management)
* Windows Command Prompt

---

## 📚 Description

Amazon S3 is an object storage service provided by AWS. In this experiment, AWS CLI is installed and configured using IAM credentials, and S3 bucket operations are performed.

---

## 🚀 Steps Performed

### 🔹 Step 1: Install AWS CLI

* Downloaded and installed AWS CLI on the local system.

---

### 🔹 Step 2: Configure AWS CLI

* Opened Command Prompt and ran:
  aws configure

* It asked for:

  * AWS Access Key
  * AWS Secret Key

---

### 🔹 Step 3: Create IAM User and Generate Keys

* Opened AWS Management Console

* Navigated to IAM service

* Created a new user

* Assigned permission: **AmazonS3FullAccess**

* Created user successfully

* Opened the user → Security Credentials

* Generated:

  * Access Key
  * Secret Access Key

* Copied both keys

---

### 🔹 Step 4: Enter Credentials in CLI

* Pasted keys in terminal
* Entered:

  * Region: ap-south-1
  * Output format: json

---

### 🔹 Step 5: Create S3 Buckets

* Created two S3 buckets using:
  aws s3 mb s3://lakshmiprasanna-s3-bucket-1 --region ap-south-1
  aws s3 mb s3://lakshmiprasanna-s3-bucket-2 --region ap-south-1

* Ensured bucket names are unique

---

### 🔹 Step 6: Verify Buckets

* Checked whether buckets are created using:
  aws s3 ls

---

### 🔹 Step 7: Delete S3 Buckets

* Deleted buckets using:
  aws s3 rb s3://lakshmiprasanna-s3-bucket-1 --force
  aws s3 rb s3://lakshmiprasanna-s3-bucket-2 --force

---

### 🔹 Step 8: Verify Deletion

* Again ran:
  aws s3 ls

* Confirmed buckets are deleted

---


## ✅ Result

Successfully installed AWS CLI, configured it using IAM credentials, created S3 buckets, verified them, and deleted them successfully.

---



## 🎬 YouTube Demo Link

https://youtu.be/TqDvbLXOL7M
