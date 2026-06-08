# Azure Arc Hybrid Management Studio

This repository contains the target configuration and SRE runtime files compiled by the **Azure Arc Hybrid Management Studio** dashboard module.

## 🚀 Description
Extend Azure control plane to external Kubernetes and bare-metal nodes. Generate onboarding scripts, policy assignments, and Azure Monitor telemetry agents bindings.

## 🛠️ Specification Matrix
- **Primary Configuration File**: `/scripts/arc_onboard.sh`
- **Execution Command**: `bash arc_onboard.sh`
- **Validation Command**: `azcmagent show`

## 📋 How to Run & Validate

1. **Clone the repository:**
   ```bash
   git clone https://github.com/Pradeeptalari14/tp-azure-arc.git
   cd tp-azure-arc
   ```

2. **Run Execution Target:**
   ```bash
   bash arc_onboard.sh
   ```

3. **Verify Runtime Stability:**
   ```bash
   azcmagent show
   ```

## 🔐 Security & Best Practices
* **Secret Isolation**: Use organization-level secrets (or SSM parameter hooks) rather than hardcoded environment variables inside files.
* **Pull Request Lifecycles**: Protect default branch merges with validation checks before merging code changes.
