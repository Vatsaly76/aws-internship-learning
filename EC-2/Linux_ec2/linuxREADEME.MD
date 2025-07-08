# 🚀 Launching a Linux Web Server on AWS EC2

This guide walks you through the process of launching a Linux EC2 instance on AWS and deploying a simple website on it.

---

- ✨  **Step 1: Go to EC2 and Launch an Instance**  
  Open the AWS Management Console, search for EC2, and click “Launch Instance”.  
  ![Step 1](step1.png)

---

- 🧩  **Step 2: Select an OS**  
  Choose an Amazon Machine Image (AMI). For this project, select Amazon Linux 2 (free tier eligible).  
  ![Step 2](step2.png)

---

- 🗝️  **Step 3: Choose Instance Type & Key Pair**  
  Pick the instance type — use t2.micro (for free tier). Then, create or select an existing key pair for SSH login.  
  ![Step 3](step3.png)

---

- 🌐  **Step 4: Configure Network Settings**  
  In the Security Group settings, enable the following:
  - SSH (port 22)
  - HTTP (port 80)
  - HTTPS (port 443)  
  This ensures your server is accessible for remote login and public website access.  
  ![Step 4](step4.png)

---

- ✅  **Step 5: Launch and Confirm Success**  
  Review your settings and click “Launch Instance”. Once successful, you’ll see your EC2 instance in the “Running” state.  
  ![Step 5](step5.png)

---

- 🔌  **Step 6: Connect to the Instance**  
  Select your running instance and click “Connect”. Use the EC2 connect option or an SSH client with your key file.  
  ![Step 6](step6.png)

---

- 💻  **Step 7: Open Linux Terminal**  
  Once connected, you'll land in a Linux shell. This is your server’s terminal where commands can be executed.  
  ![Step 7](step7.png)

---

- ⚙️  **Step 8: Write Linux Commands**  
  You will now update the server, install the Apache web server, and start the service so it can serve web pages.  
  ![Step 8](step8.png)

---

- 📝  **Step 9: Add Your Website Code**  
  After setting up Apache, you create an HTML file with your website content. This file is placed inside the default web directory of the server. It acts as your homepage and will be served to anyone who accesses your instance’s IP address.  
  ![Step 9](step9.png)

---

- 🌍  **Step 10: Visit Website Using Public IP**  
  Return to the EC2 dashboard, copy your instance's Public IPv4 address, and open it in any web browser. Your website, hosted from your Linux EC2 instance, should now be live and accessible over the internet.  
  ![Step 10](step10.png)

---

🎉  Great Job! You’ve successfully launched and deployed a live Linux-based website using Amazon EC2.
