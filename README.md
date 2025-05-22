# ☁️ Cloud IAM & Least Privilege Lab – GCP + Terraform

A hands-on cloud security project to explore and enforce **Identity and Access Management (IAM)** principles using **Google Cloud Platform (GCP)** and **Terraform**. This lab demonstrates how to provision infrastructure securely, apply least privilege access, simulate misconfigurations, and analyze permission behaviors—all through code.

---

## 📌 Project Objective

This lab was created as part of my **2025 Cloud Security learning roadmap** to gain real-world experience in:
- Managing IAM roles, service accounts, and permissions in GCP
- Applying least privilege using Infrastructure as Code (IaC)
- Identifying, simulating, and correcting IAM misconfigurations
- Preparing for future certifications and cloud security roles

---

## 🛠️ Tools & Technologies

- **Google Cloud Platform (GCP)** – Compute, IAM, Cloud Storage
- **Terraform** – Infrastructure as Code
- **gcloud CLI** – GCP authentication and management
- **Linux Ubuntu VM** (Compute Engine)
- **GitHub** – Documentation, IaC version control

---

## 🎯 Lab Goals

- ✅ Deploy secure infrastructure using Terraform
- ✅ Create and assign custom IAM roles to service accounts
- ✅ Apply least privilege enforcement across services
- ✅ Simulate IAM misconfigurations and debug using GCP tools
- ✅ Validate access via CLI and service account impersonation
- ✅ Document and share learning through GitHub

---

## 📅 7-Day Plan (Progress Tracker)

### ✅ Day 1–2: Environment Setup & GCP Project Initialization
- Create new GCP project (Free Tier)
- Enable required APIs: IAM, Compute Engine, Cloud Storage
- Set up local Terraform CLI and authenticate via `gcloud`
- Initialize GitHub repo with project folders

### ⏳ Day 3: Deploy GCP VM and Basic IAM Roles via Terraform
- Create Ubuntu VM and basic service account via `main.tf`
- Assign Viewer role and test access through SSH
- Document and verify permission boundaries

### ⏳ Day 4: Implement and Test Least Privilege IAM
- Replace default roles with custom or scoped roles
- Assign `storage.objectViewer` and test what’s allowed/denied
- Record SPL-like output (logs/errors) from GCP CLI

### ⏳ Day 5: Simulate IAM Misconfigurations
- Over-assign (Owner), then under-assign (no access)
- Use **Policy Troubleshooter** to identify cause of denial
- Screenshot error states and debugging process

### ⏳ Day 6: Add Cloud Storage + RBAC Validation
- Create a GCS bucket and attach IAM roles via Terraform
- Test:
  - Upload = ✅?
  - Delete = ❌?
- Validate that permissions behave as expected

### ⏳ Day 7: Cleanup + GitHub Documentation
- Finalize and clean up Terraform files
- Add screenshots and test logs
- Push complete lab to GitHub
- Prepare summary for LinkedIn or blog

---

## 📂 Project Structure

```plaintext
cloud-iam-lab/
├── README.md
├── /terraform
│   ├── main.tf
│   ├── variables.tf
│   └── outputs.tf
├── /screenshots
│   ├── iam-policy-success.png
│   ├── access-denied-debug.png
├── /docs
│   └── policy_testing_notes.md

---

## 🔐 What I Learned

- How GCP IAM works: roles, bindings, service accounts  
- How to restrict and validate permissions using least privilege  
- How Terraform enables version-controlled cloud security  
- How to simulate IAM issues and troubleshoot access  
- How to structure cloud security labs for GitHub portfolios  

---

## 🚀 Future Enhancements

- Add organization policies (e.g., disable default service accounts)  
- Integrate GCP Audit Logs for access monitoring  
- Extend to multi-cloud (Azure AD, AWS IAM)  
- Compare GCP IAM with AWS IAM and Azure RBAC  
- Build alerting rules around access violations  

---

## 📣 Acknowledgements

This project is part of my **2025 Core Skills Year** toward cloud security specialization.  
Inspired by hands-on labs and blue team best practices from **Security Blue Team** and **Google Cloud documentation**.

---
