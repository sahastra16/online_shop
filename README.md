Project Name: 🚀 Hackathon Phase-1: Mastering Linux, GitHub & Docker! 🔥
💡 Challenge Accepted: Participating in TrainWithShubham.com’s Hackathon Phase-1 was an intense learning experience, pushing us to deploy an application from scratch using Linux, GitHub, and Docker. Here’s a breakdown of our journey—what worked, what didn’t, and how we overcame it! ✅

🔍 Case Study: Overcoming Docker Build Issues & Clean Code Practices
Step 1: Setting Up the AWS Environment
🔹 Launched an EC2 instance (Ubuntu)
🔹 Configured security groups for SSH (22), HTTP (80), and HTTPS (443)
🔹 Connected via SSH & updated system packages

Step 2: Installing Required Dependencies
🔹 Installed Docker, Node.js, and Git
🔹 Verified installations (docker -v, node -v, git --version)

Step 3: Cloning the GitHub Repository
🔹 Used git clone <repo_url> to fetch source code
🔹 Identified package.json for dependencies and libraries
🔹 Reviewed the project structure for missing dependencies

Step 4: Fixing Docker Build Issues
🔍 Challenges Encountered:
❌ EJSONPARSE error in package.json due to comments
❌ Permission Denied when running docker build
❌ Missing dependencies leading to installation failures

✅ Solutions Implemented:
🔹 Removed invalid JSON comments to fix parsing errors
🔹 Used chmod +x entrypoint.sh to fix executable permissions
🔹 Ran npm install --legacy-peer-deps to resolve package conflicts

Step 5: Building & Running Docker Container
🔹 Used docker build -t my-app . to build the image
🔹 Started the container with docker run -d -p 80:3000 my-app
🔹 Verified running containers with docker ps

Step 6: Accessing the Application via Public IP
🔹 Retrieved the EC2 Public IP
🔹 Opened the browser to http://<Public-IP> & tested the deployment

Key Takeaways:
✅ Understanding package dependencies to avoid build failures
✅ Keeping package.json clean and error-free 🔍
✅ Fixing Docker-related issues proactively 💡
✅ Committing structured & optimized code to GitHub 🔥

A visual representation of this workflow is attached below! 📌

👉 Have you faced similar challenges while deploying an app? Let’s discuss in the comments! 💬

