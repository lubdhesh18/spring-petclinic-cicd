![Jenkins](https://img.shields.io/badge/Jenkins-Automation-red)
![SonarQube](https://img.shields.io/badge/SonarQube-Code%20Quality-blue)
![Nexus](https://img.shields.io/badge/Nexus-Repository-orange)
![Tomcat](https://img.shields.io/badge/Tomcat-10-yellow)
![AWS](https://img.shields.io/badge/AWS-EC2-brightgreen)
![Maven](https://img.shields.io/badge/Maven-Build-lightgrey)

# 🚀 Spring PetClinic – Complete CI/CD Pipeline (Jenkins | SonarQube | Nexus | Tomcat | AWS)

This project demonstrates a **full CI/CD pipeline** for the Spring PetClinic application using modern DevOps tools.  
It covers the complete lifecycle: **Build → Test → Analyze → Store → Deploy**.

---

## 🧰 **Tech Stack**

| Tool | Purpose |
|------|---------|
| 🟦 Jenkins | CI/CD Pipeline Automation |
| 🐳 AWS EC2 | Hosting Jenkins, SonarQube, Nexus, Tomcat |
| ✔️ Maven | Build & Dependency Management |
| 🔍 SonarQube | Code Quality & Static Analysis |
| 📦 Nexus Repository | Artifact Storage (WAR) |
| 🐱 Tomcat 10 | Deployment Server |
| ☕ Java / Spring | Application Framework |

---

## 🎯 **Pipeline Flow (High-Level Architecture)**
GitHub → Jenkins → SonarQube → Maven Build → Nexus → Tomcat Deployment

<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/b290e882-6e01-49fb-abd4-f6d9e6e6ec8e" />


---

## 🚦 **CI/CD Pipeline Stages**

### **1️⃣ Source Stage**
- Jenkins pulls the PetClinic repo from GitHub  
- Triggered by a webhook or manual build

### **2️⃣ Code Quality Check**
- SonarQube scanner runs
- Quality Gate must pass to continue

### **3️⃣ Build Stage**
- Maven compiles the project  
- Packages the `.war` file  

### **4️⃣ Upload to Nexus**
- WAR is uploaded to Nexus Repository  
- Stored with versioning (`6.2.8` etc.)

### **5️⃣ Deployment**
- Jenkins copies the artifact to Tomcat 10  
- Auto deploys to:  
  👉 `http://<tomcat-ip>:8080/petclinic`

---

## 📊 **Pipeline Screenshot Highlights**
(All images go into `/screenshots/` folder)

- ✔️ Jenkins Pipeline Success  
- 🔍 SonarQube Code Quality Report  
- 📦 Nexus Artifact Upload  
- 🐱 Tomcat Deployment (Live App)  
- 🖥️ EC2 Instances Setup

---

## 📦 **Nexus Configuration**

Repository: maven-releases

Group ID: org.springframework.samples

Artifact: spring-framework-petclinic

Version: 6.2.8

## 🔐 **EC2 Setup Summary**

| Instance  | Purpose                |
| --------- | ---------------------- |
| Jenkins   | Pipeline automation    |
| SonarQube | Code quality           |
| Nexus     | Artifact repository    |
| Tomcat    | Application deployment |

## 🌐 **Live Application Screenshot**
See /screenshots/DeployedTomcat10/

## 🏁 **Final Output**

✔️ Fully automated CI/CD pipeline

✔️ Quality gate validation

✔️ Artifact lifecycle management

✔️ Zero manual deployment

✔️ Professional DevOps project ready for portfolio & resume

## ⭐ **If this project helped you, give it a star!**
