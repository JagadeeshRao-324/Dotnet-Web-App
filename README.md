

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
| Dev   | Deploy to Dev App Service      | `dotnetapp-dev`  |
| QA    | Deploy to QA App Service       | `dotnetapp-qa`   |
| Prod  | Deploy to Production App       | `dotnetapp-prod` |

---


