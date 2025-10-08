# 🌩️ CI/CD Resume Pipeline on AWS

This project demonstrates a **two-stage CI/CD pipeline** using **GitHub** and **AWS CodePipeline** to deploy a **static resume website** displaying my resume hosted on **Amazon S3** with **CloudFront HTTPS** and a custom domain.

---

## 🚀 Project Overview

- **Source Control:** GitHub  
- **CI/CD Service:** AWS CodePipeline  
- **Hosting:** Amazon S3 (Static Website Hosting)  
- **Security:** HTTPS via CloudFront + Route 53  
- **Website Content:** index.html + style.css (Resume Page)

---

## 🧩 Steps Followed

### 1. Local Project Setup
- Created project folder `resume-pipeline`
- Added `index.html` and `style.css`,image
- Initialized Git and pushed to GitHub repository
<img width="1920" height="981" alt="Screenshot (427)" src="https://github.com/user-attachments/assets/c678ddf3-3ebe-4f23-b041-aaf9f88319c0" />


### 2. S3 Bucket Configuration
- Created an S3 bucket: `resume-pipeline-bucket`
- Enabled static website hosting  
- Added bucket policy to allow public access  
<img width="1920" height="954" alt="Screenshot (409)" src="https://github.com/user-attachments/assets/8ce242b0-fe91-40ad-828d-1d4d3fc798ad" />

### 3. Pipeline Setup
- Created a two-stage AWS CodePipeline  
- Source: GitHub repository  
- Deploy: S3 bucket  
- Automated deployment triggered
<img width="1920" height="966" alt="Screenshot (410)" src="https://github.com/user-attachments/assets/67796595-b0a2-41f0-aef6-5b17cd63b119" />
- files on the remote repo that contain what will display on the website will automated and stored in the S3 bucket
  <img width="1920" height="978" alt="Screenshot (428)" src="https://github.com/user-attachments/assets/7b70c9b1-f0c1-45ed-9d34-ded9c4f57fbe" />

### 4. Security Enhancement
- Request an SSL/TLS Certificate in ACM
  <img width="1920" height="966" alt="Screenshot (413)" src="https://github.com/user-attachments/assets/ee902250-64d0-47f1-9c3a-0ae9782b0cc3" />

- Integrated CloudFront for HTTPS
   <img width="1920" height="960" alt="Screenshot (416)" src="https://github.com/user-attachments/assets/9fa3b15d-e62b-4aa6-9f4d-c90d179c1a01" />
- Update bucket policy so cloud front can access the bucket privately
  <img width="1920" height="981" alt="Screenshot (417)" src="https://github.com/user-attachments/assets/a51752fe-5955-4df3-aa2c-f1a269a87876" />

- Linked Route 53 domain: `resume.anzyworld.com`
  <img width="1920" height="944" alt="Screenshot (419)" src="https://github.com/user-attachments/assets/8f0ee103-ce6e-41b2-97cc-104d84b37653" />

### 5. Test the website.

 <img width="1920" height="950" alt="Screenshot (430)" src="https://github.com/user-attachments/assets/8d44c3f9-aac7-47e8-b95b-1e6b0c6e1b80" />

- checking to see if its secured as well.
  <img width="1920" height="973" alt="Screenshot (431)" src="https://github.com/user-attachments/assets/370c2147-29d3-4234-bd80-f387a0161a39" />





## 🔗 Live Website

👉(https://resume.anzyworld.com)


## 🧰 Technologies Used
- AWS S3  
- AWS CodePipeline  
- AWS CloudFront  
- Route 53  
- GitHub  
- HTML / CSS  

---

## 🏁 Conclusion
This project successfully implements a **CI/CD pipeline** that automates static website deployment.  
It demonstrates continuous delivery, domain integration, and secure HTTPS hosting on AWS.
