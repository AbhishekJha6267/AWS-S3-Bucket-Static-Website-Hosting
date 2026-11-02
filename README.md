☁️ AWS S3 Bucket Static Website Hosting
📌 Project Overview

This project demonstrates how to host a static website using Amazon Web Services (AWS) S3 (Simple Storage Service).

The objective is to deploy a personal portfolio website on Amazon S3 and make it accessible through a public website endpoint without managing any servers.

This project provides hands-on experience with AWS cloud infrastructure, S3 bucket configuration, static website hosting, and bucket access permissions.

🎯 Project Objectives
Create and configure an Amazon S3 bucket.
Upload static website files to S3.
Enable static website hosting.
Configure bucket permissions using an S3 bucket policy.
Make the website publicly accessible.
Access the hosted website through the S3 website endpoint.
🛠️ Technologies Used
AWS S3 – Static website hosting and file storage.
HTML5 – Website structure.
CSS3 – Website styling and responsive layout.
JSON – S3 bucket access policy.
AWS Management Console – Cloud resource configuration.
🏗️ Project Architecture

The project follows a simple static website hosting architecture:

text
          User / Browser
                |
                |
                v
       Amazon S3 Website URL
                |
                |
                v
          S3 Bucket
                |
                |
         +------+------+
         |             |
         v             v
      index.html   Other Assets
         |
         v
    Static Website

📂 Repository Structure
text
AWS-S3-Bucket-Static-Website-Hosting/
│
├── Screenshot's/
│   └── AWS project screenshots
│
├── bukcet_policy.json
│
├── index.html
│
└── README.md

⚙️ Implementation Steps
Step 1: Create an S3 Bucket
Log in to the AWS Management Console.
Navigate to Amazon S3.
Click on Create bucket.
Enter a globally unique bucket name.
Select your preferred AWS Region.
Configure public access settings according to your hosting approach.
Create the bucket.
Step 2: Upload Website Files
Open the newly created S3 bucket.
Navigate to the Objects section.
Click Upload.
Upload the index.html file.
Upload any additional website assets.
Complete the upload.
Step 3: Enable Static Website Hosting
Open the bucket's Properties tab.
Navigate to Static website hosting.
Select Enable.
Choose Host a static website.
Set index.html as the Index document.
Save the configuration.
Step 4: Configure Bucket Permissions
Navigate to the Permissions tab.
Open the Bucket Policy section.
Configure the appropriate permissions for reading website objects.
Save the bucket policy.

Note: For a public S3 website endpoint, the bucket must allow public read access, and S3 Block Public Access settings must be configured accordingly. Public access should only be enabled intentionally for this demonstration.

Step 5: Access the Hosted Website
Navigate to the Properties tab.
Find the Static website hosting section.
Copy the Bucket website endpoint.
Open the endpoint in your browser.

Your static website should now be accessible!

📸 Project Screenshots

Screenshots demonstrating the AWS S3 configuration and website deployment are available in the Screenshot's directory.

🔐 Security Considerations
Avoid uploading sensitive information or credentials.
Follow the principle of least privilege.
Do not grant unnecessary write or delete permissions.
Public bucket access should be enabled only when required.
For production websites, consider using Amazon CloudFront with Origin Access Control and a private S3 bucket.
📚 Key Learnings

Through this project, I gained practical knowledge of:

AWS S3 bucket creation and management.
Static website hosting on AWS.
Website deployment using cloud storage.
S3 bucket policies and IAM-related access concepts.
Public access configuration.
Hosting static websites without provisioning EC2 instances.
🚀 Future Improvements
Integrate Amazon CloudFront for content delivery.
Configure a custom domain using Amazon Route 53.
Enable HTTPS using AWS Certificate Manager.
Automate deployment using AWS CLI or CI/CD pipelines.
👨‍💻 Author

Abhishek Jha

Aspiring Cloud Engineer | AWS | Linux | DevOps

GitHub: AbhishekJha6267

⭐ If you find this project useful, feel free to star the repository!

Thank you for visiting!
