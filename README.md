

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

Project Setup :

1. Imported the ASP.NET app code from https://github.com/MicrosoftDocs/pipelines-dotnet-core.git to my azure repos.
2. Established the connection to SonarQube cloud and Azure cloud using service connections.
3. Created the DEV, QA and PROD environments with pre-approval checks
4. Built the CI/CD pipeline.
5. CI pipeline builds, packages, and publishes the artifact to pipeline workspace and generates the SAST code scan reports in SonarQube
6. CD pipeline downloads the artifact and deploys it to the azure web app service across dev, qa, and prod.
   

![Image](https://github.com/user-attachments/assets/89ea7863-aef4-453c-8e55-b7a09ae97f5b)

