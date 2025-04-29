## ⚙️ Terraform GitHub Module — Features

This module automates the complete setup of a GitHub repository using Terraform.

---

### 📦 What It Does

- Creates a GitHub repository
- Creates and manages branches:
  - `main` (default, protected)
  - `dev`, `qa`, `ppd`, `dr`, `ci`
- Configures branch protection rules:
  - Enforces admin restrictions
  - Requires PR reviews
  - Enables status checks: `ci`, `lint`, `security`
  - Disables force-push and deletions
- Creates GitHub Actions environments:
  - `main`, `dev`, `qa`, `ppd`, `dr`, `ci`, `integration`
- Adds environment-level variables and secrets
- Adds collaborators with permission levels
- Creates custom issue labels
- Adds repository webhooks
- Uploads custom files (e.g. `.github/workflows/*.yml`)

---

### 🔐 Security & DevOps Automation

- Branch protection enabled by default
- CI/CD ready: `fmt`, `validate`, `tflint`, `checkov`, `trivy`
- Dependabot auto-updates for Terraform & GitHub Actions
- Includes `verify.py` to validate Terraform vs live GitHub state
