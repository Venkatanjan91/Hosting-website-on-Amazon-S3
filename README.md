#  🚀 Host a Website on Amazon S3

## 📌 Introduction
⚡📦 **Amazon S3**(Simple Storage Service) 🔒💡💻 is a scalable, secure, and durable cloud storage service used for various purposes such as 📦 storage, 🔄 backups, 🌍 hosting, 📊 analytics, 🚀 content delivery, 🛑 disaster recovery, and 🤖 machine learning datasets.

## 🌐 Project Overview
In this project, Amazon S3 🌍📡 was used to host a static website by enabling Static Website Hosting 🛠️💾, uploading HTML and other assets, and configuring permissions for public access.

### ⚠️ Unexpected Challenge
⚡ One challenge faced was that even after enabling Static Website Hosting, the uploaded files remained private by default because Amazon S3 does not make objects public automatically for security reasons. 🛠️ Manual updates ⚙️🔧 to bucket policies 📑 and ACLs 🏗️🔍 were required to make them publicly accessible 🌎🔓🚀.

## ⏳ Project Duration
⏱️ Setting up the S3 bucket 🗂️, enabling static website hosting 🌐, and uploading files 📤📂 took approximately 15-20 minutes ⌛.. However, additional time was required to configure permissions and troubleshoot access issues.

## 🛠️ Steps to Set Up an S3 Bucket

### 📂 Create an S3 Bucket

* Go to the **AWS S3** Management Console.

* Click **Create bucket**.

* Enter **Bucket Name** (must be unique across AWS).

* Select **Region** (choose the closest or required AWS region).

* The selected AWS region was **Asia Pacific (Mumbai) - ap-south-1** (chosen for proximity).

* S3 **bucket names must be globally unique** to ensure distinct identification across AWS accounts and regions.

![Creating a Bucket](https://github.com/user-attachments/assets/35229f1b-787b-4bc8-9aa8-41ca1b11501f)

### 📤 Upload Website Files to S3

* The uploaded files 📄 included index.html and NextWork - Everyone should be in a job they love_files.zip 📦.

* The HTML file serves as the main webpage, while the ZIP file likely contains assets such as images, CSS, JavaScript, or additional pages.
* 
![Upoad the HTML and Zip files](https://github.com/user-attachments/assets/cb6b62b6-f955-4a04-9a2e-2a21423f6f09)

### 🌍 Enable Static Website Hosting

* Web hosting involves storing and serving website files online.

* To enable website hosting with my S3 bucket, I went to **Properties** > **Static website hosting**, chose Edit, enabled hosting, set Hosting type to **"Host a static website"**,and entered index.html as the Index document.

* Access Control Lists (ACLs) were enabled to manage access control for uploaded objects.

![Enable Static Website Hosting](https://github.com/user-attachments/assets/9dd0d82d-c397-4096-aa4a-fa8b8a0911c3)

### 🔗 Bucket Endpoints

* 🔗 Enabling static website hosting generates a bucket endpoint URL, which is a public link to access the site via HTTP.

* ⚠️ Initially, accessing the URL 🚫🔗 resulted in a **403 Forbidden error ❌🚷** because the bucket's objects were private by default. **AWS requires explicit permission settings**, such as **bucket policies or ACL updates**, to make files publicly accessible.

![Bucket Endpoints](https://github.com/user-attachments/assets/d06d164a-b044-4d0b-8041-098816a97f78)

### 🌐 Making the Website Public

* To resolve the issue, the following steps were taken:

* Navigate to the **Objects** tab.

* Select the **checkboxes** next to index.html and the folder containing website assets.

* In the **Actions** dropdown, choose **Make public using ACL**.

![Making the Website Public](https://github.com/user-attachments/assets/bc74434c-5205-4e88-9b21-b8c4a56209c8)

## ✅ Conclusion
🎉🔑 After configuring the required permissions 🔐✅, the website 🌎🌍 was successfully hosted 🏆🎯 on Amazon S3 🚀🔥.. This project demonstrated how to set up, configure, and troubleshoot an S3-hosted static website.
*  https://venkatanjan91.github.io/Hosting-website-on-Amazon-S3/
