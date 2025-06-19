

# ASP.NET WebApp CI/CD Pipeline with Azure DevOps


This repository contains a **.NET 8.0 Web Application** with a complete **multi-stage CI/CD pipeline** built using **Azure DevOps**. The pipeline implements:

- 🔨 Build & Restore
- 🧪 Code Quality Checks using **SonarQube Cloud**
- 📦 NuGet Packaging & Publishing to **Azure Artifacts**
- 🚀 Multi-Stage Deployment to **Azure App Service** across **Dev**, **QA**, and **Prod** environments

---

## 🌐 Environments

| Stage | Description                    | Environment      |
|-------|--------------------------------|------------------|
| Build | Build, test, analyze, publish  | Agent workspace  |
| Dev   | Deploy to Dev App Service      | `DEV`  |
| QA    | Deploy to QA App Service       | `QA`   |
| Prod  | Deploy to Production App       | `PROD` |

---

![Image](https://github.com/user-attachments/assets/89ea7863-aef4-453c-8e55-b7a09ae97f5b)

