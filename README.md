# 📌 DevOps Internship — Task 8
  ⚙️ Building & Running a Java Maven Project with Jenkins Pipeline
  📖 Project Description

In this task, I created a Java Maven project (HelloWorld) and automated its build process using Jenkins Pipeline.
The application prints a simple output:

```bash
Hello, Jenkins + Maven!
```

The project was compiled and packaged using Maven (with the Shade plugin for an executable JAR), and the CI/CD process was handled by a Jenkins Pipeline job.

All steps are supported with screenshots for clarity and evaluation.

# 📊 Execution Evidence & Screenshots

## 📂 1. Project Structure in VS Code

Description: Organized the Java project with the proper Maven directory layout under src/main/java. Added the pom.xml build file with the Shade plugin to ensure an executable JAR with the correct Main-Class.
📷 Screenshot: VS Code Explorer showing HelloWorld.java, pom.xml, and Jenkinsfile in correct structure.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/88b5f308-71d7-43a3-8818-b34cdbcc05ff" />


## 📝 2. Java HelloWorld Application

Description: Implemented the main class inside the package com.example.app. The class prints a confirmation message.
📷 Screenshot: Code editor showing HelloWorld.java content.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/960f57dd-22d5-499c-a268-2249d584a634" />

## 📦 3. Maven Build Success (Local)

Description: Ran mvn clean package locally to verify compilation and JAR creation. Confirmed JAR contains HelloWorld.class and proper Main-Class in manifest.
📷 Screenshot: Terminal output of Maven build success with JAR created under target/.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ceb00ea3-2162-4d2a-8427-a41fc4e45eb5" />


🔧 4. Jenkins Global Tool Configuration

Description: Configured Maven (Maven-3.8) inside Global Tool Configuration so Jenkins Pipeline could invoke mvn.
📷 Screenshot: Jenkins → Global Tool Configuration page showing Maven installation.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/1155c46c-d9fa-455c-94f5-1037d1cd9cd0" />


📜 5. Jenkins Pipeline Job Configuration

Description: Created a Pipeline job named jenkins-maven-build, linked it to the GitHub repository, and pointed to the Jenkinsfile.
📷 Screenshot: Jenkins job configuration page (Pipeline script from SCM with repo URL).

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/3c17c28c-9cbc-48f4-9659-dffd420b13ff" />


🚀 6. Jenkins Build Execution (Console Output)

Description: Ran the pipeline job which checked out the repo, built the JAR using Maven, verified its contents, and archived artifacts. Build completed successfully.
📷 Screenshot: Console Output page showing BUILD SUCCESS and manifest details.

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/30b49b9b-c7d6-492c-87d6-8b87bd8bca7c" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/ea0ecdd2-4dd6-46f5-89d5-5188e83c124c" />


📑 Final Deliverables

✅ Java Maven source code (HelloWorld.java)
✅ pom.xml with Shade plugin for executable JAR
✅ Jenkinsfile (Windows-compatible with Maven tool)

🌟 Key Learnings

-Understood how to properly structure a Maven project with Java packages.
-Learned how to configure Jenkins Global Tools (Maven, JDK).
-Gained hands-on practice with Jenkins Pipeline scripts.
-Debugged common issues like ClassNotFoundException due to incorrect package structure and missing Main-Class in the JAR manifest.
-Automated build lifecycle from GitHub → Jenkins → Maven build → Artifact archive.

🙏 Acknowledgement

I sincerely thank my mentor and the DevOps internship team for their constant guidance throughout this task.
Special thanks to the open-source community behind Jenkins and Maven for enabling modern CI/CD workflows.

Submitted by: Deepak Jaiswal
Date: 03/10/2025
