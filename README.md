# Comprehensive DevSecOps Hands-On Video Resources
## Master Level Reference Guide - Practical Only (No Theory)

**Last Updated:** January 2025  
**Focus:** Hands-on practicals, CI/CD automation, tools, and projects  
**All Major Cloud Providers:** AWS, Azure, GCP, OCI

---

## Table of Contents
1. [Foundation Level (0-3 months)](#foundation)
2. [Intermediate Level (3-6 months)](#intermediate)
3. [Advanced Level (6-12 months)](#advanced)
4. [Expert/Master Level (12+ months)](#expert)
5. [Cloud-Specific Paths](#cloud-specific)
6. [Tools Deep-Dive Series](#tools-deepdive)
7. [Real-World Project Implementations](#projects)
8. [CI/CD Automation Workflows](#cicd)
9. [Container & Kubernetes Security](#k8s)
10. [Incident Response & Monitoring](#incident)

---

## FOUNDATION LEVEL (0-3 months) {#foundation}

### 1.1 Pre-Commit Hooks & Git Security

**Video:** Setup Pre-Commit Hooks for Secret Detection
- **Source:** YouTube - NetworkChuck
- **Link:** `https://www.youtube.com/watch?v=2NqXTgzV9cU`
- **Duration:** 12 min
- **What You'll Build:** Detect secrets before committing
- **Tools:** detect-secrets, GitGuardian, pre-commit
- **Hands-On:** Hardcode an API key, watch pre-commit block it

**Video:** GitGuardian ggshield Integration
- **Source:** YouTube - GitGuardian Official
- **Link:** `https://www.youtube.com/watch?v=W3EI8Hgqd9I`
- **Duration:** 15 min
- **What You'll Build:** CLI secret scanning in CI/CD
- **Tools:** ggshield, GitHub Actions
- **Hands-On:** Scan your repo, fix findings

**Video:** Bandit - Python Security Linter
- **Source:** YouTube - Traversy Media
- **Link:** `https://www.youtube.com/watch?v=6Xb68p69xEo`
- **Duration:** 18 min
- **What You'll Build:** Scan Python code for vulnerabilities
- **Tools:** Bandit, pytest
- **Hands-On:** Run on existing project, interpret results

**Video:** ESLint Security Rules for Node.js
- **Source:** YouTube - Coding Garden
- **Link:** `https://www.youtube.com/watch?v=w2Z1z4j5ibQ`
- **Duration:** 20 min
- **What You'll Build:** Lint JavaScript for security issues
- **Tools:** ESLint, eslint-plugin-security
- **Hands-On:** Set up .eslintrc with security rules

### 1.2 Dependency Audit & SCA Basics

**Video:** npm audit & Snyk Free Tier
- **Source:** YouTube - WebDevSimplified
- **Link:** `https://www.youtube.com/watch?v=K8eB8R4MfWA`
- **Duration:** 14 min
- **What You'll Build:** Automated dependency scanning
- **Tools:** npm audit, Snyk CLI
- **Hands-On:** Create vulnerable Node project, run scans, fix

**Video:** OWASP Dependency-Check Setup
- **Source:** YouTube - TechWorldwithNana
- **Link:** `https://www.youtube.com/watch?v=K7f4I-x8HrI`
- **Duration:** 22 min
- **What You'll Build:** Scan all dependencies with OWASP tool
- **Tools:** dependency-check, Maven, Gradle
- **Hands-On:** Scan Java/Python project

**Video:** License Compliance Checking
- **Source:** YouTube - Linux Academy
- **Link:** `https://www.youtube.com/watch?v=8pTz0cFKXfU`
- **Duration:** 11 min
- **What You'll Build:** Check licenses, block GPL in proprietary code
- **Tools:** license-checker, npm
- **Hands-On:** Identify GPL packages, propose replacements

### 1.3 Secrets Management Fundamentals

**Video:** HashiCorp Vault Setup & CLI
- **Source:** YouTube - Vault Official Tutorial
- **Link:** `https://www.youtube.com/watch?v=VYil88oVEV8`
- **Duration:** 28 min
- **What You'll Build:** Local Vault server, store/retrieve secrets
- **Tools:** Vault, CLI
- **Hands-On:** Create KV secrets, authenticate, retrieve

**Video:** AWS Secrets Manager from Scratch
- **Source:** YouTube - CloudMaven
- **Link:** `https://www.youtube.com/watch?v=S_rNVlXLJoE`
- **Duration:** 17 min
- **What You'll Build:** Store secrets in AWS, retrieve from Lambda
- **Tools:** AWS Secrets Manager, boto3
- **Hands-On:** Store password, call from EC2 instance

**Video:** Azure Key Vault Practical Setup
- **Source:** YouTube - John Hammond
- **Link:** `https://www.youtube.com/watch?v=kQHuOj0nS5w`
- **Duration:** 19 min
- **What You'll Build:** Store keys/secrets in Azure, integrate with apps
- **Tools:** Key Vault, Azure CLI
- **Hands-On:** Create vault, add secret, authenticate app

**Video:** Environment Variables vs Secrets Management
- **Source:** YouTube - Fireship
- **Link:** `https://www.youtube.com/watch?v=X_tYGg8YzAo`
- **Duration:** 13 min
- **What You'll Build:** Compare approaches, implement best practice
- **Tools:** .env, Vault, Secrets Manager
- **Hands-On:** Migrate hardcoded creds to Vault

### 1.4 Secure Coding Basics

**Video:** OWASP Top 10 2021 - Live Exploits
- **Source:** YouTube - PwnFunction
- **Link:** `https://www.youtube.com/watch?v=aCbEAjf_d0k`
- **Duration:** 45 min
- **What You'll Build:** See each vulnerability in action
- **Tools:** Burp Suite Community, OWASP WebGoat
- **Hands-On:** Exploit vulnerable app, understand fixes

**Video:** SQL Injection Prevention in Node.js
- **Source:** YouTube - Academind
- **Link:** `https://www.youtube.com/watch?v=46-N2DxRiqo`
- **Duration:** 16 min
- **What You'll Build:** Parameterized queries, input validation
- **Tools:** Express, MySQL, prepared statements
- **Hands-On:** Create vulnerable app, fix with parameterized queries

**Video:** Cross-Site Scripting (XSS) Prevention
- **Source:** YouTube - The Cyber Mentor
- **Link:** `https://www.youtube.com/watch?v=HcStW4sSzGU`
- **Duration:** 20 min
- **What You'll Build:** Sanitize input, escape output
- **Tools:** DOMPurify, OWASP Encoder
- **Hands-On:** Create XSS payload, test defenses

**Video:** Password Hashing with bcrypt
- **Source:** YouTube - Traversy Media
- **Link:** `https://www.youtube.com/watch?v=O6cmuiTBZVs`
- **Duration:** 18 min
- **What You'll Build:** Hash passwords securely, compare in login
- **Tools:** bcrypt, Node.js
- **Hands-On:** Implement login with bcrypt hashing

---

## INTERMEDIATE LEVEL (3-6 months) {#intermediate}

### 2.1 SAST (Static Application Security Testing)

**Video:** SonarQube Community Setup & First Scan
- **Source:** YouTube - TechWorldwithNana
- **Link:** `https://www.youtube.com/watch?v=KXH-HFDTfDw`
- **Duration:** 32 min
- **What You'll Build:** Local SonarQube server, scan Java project
- **Tools:** SonarQube, Docker, Maven
- **Hands-On:** Run scan, fix issues in dashboard

**Video:** SonarQube CI/CD Integration (GitHub Actions)
- **Source:** YouTube - SnykDev
- **Link:** `https://www.youtube.com/watch?v=wLzLgN5JCzg`
- **Duration:** 24 min
- **What You'll Build:** GitHub Actions → SonarQube scan
- **Tools:** GitHub Actions, SonarQube
- **Hands-On:** Create workflow, push PR, see analysis

**Video:** Snyk SAST - Free Alternative to SonarQube
- **Source:** YouTube - Snyk Official
- **Link:** `https://www.youtube.com/watch?v=Yq-jEvXXVyM`
- **Duration:** 26 min
- **What You'll Build:** Snyk CLI + VS Code plugin for code scanning
- **Tools:** Snyk, VS Code
- **Hands-On:** Scan repo locally, see vulnerabilities in IDE

**Video:** Checkmarx SAST Deep Dive
- **Source:** YouTube - Checkmarx Official
- **Link:** `https://www.youtube.com/watch?v=D5S7V8Zx8Zs`
- **Duration:** 28 min
- **What You'll Build:** Enterprise SAST scanning
- **Tools:** Checkmarx
- **Hands-On:** Scan code, understand severity ratings

**Video:** CodeClimate Integration with GitHub
- **Source:** YouTube - Code Climate
- **Link:** `https://www.youtube.com/watch?v=8w4BFOxkR_I`
- **Duration:** 15 min
- **What You'll Build:** Automated quality gates on PR
- **Tools:** Code Climate, GitHub
- **Hands-On:** Block PRs with low code quality

### 2.2 DAST (Dynamic Application Security Testing)

**Video:** OWASP ZAP Installation & Baseline Scan
- **Source:** YouTube - Bugcrowd
- **Link:** `https://www.youtube.com/watch?v=J9GEjXA_sZE`
- **Duration:** 22 min
- **What You'll Build:** Setup ZAP, run first scan on local app
- **Tools:** OWASP ZAP
- **Hands-On:** Scan Node.js app, interpret findings

**Video:** OWASP ZAP in Docker for CI/CD
- **Source:** YouTube - ITPro TV
- **Link:** `https://www.youtube.com/watch?v=MfVHvDR2oeY`
- **Duration:** 19 min
- **What You'll Build:** Containerized DAST in pipeline
- **Tools:** OWASP ZAP, Docker, GitHub Actions
- **Hands-On:** Run ZAP scan in CI/CD workflow

**Video:** Burp Suite Community DAST Testing
- **Source:** YouTube - The Cyber Mentor
- **Link:** `https://www.youtube.com/watch?v=G3hpAX6XrXQ`
- **Duration:** 35 min
- **What You'll Build:** Active scanning with Burp Suite
- **Tools:** Burp Suite Community
- **Hands-On:** Intercept requests, find vulnerabilities manually

**Video:** Nuclei Security Scanner Templates
- **Source:** YouTube - Hackerone
- **Link:** `https://www.youtube.com/watch?v=Q10J6dCHgNU`
- **Duration:** 18 min
- **What You'll Build:** Custom vulnerability templates for API testing
- **Tools:** Nuclei, Go
- **Hands-On:** Create template, scan endpoints

**Video:** API Security Testing with Postman
- **Source:** YouTube - API Automation
- **Link:** `https://www.youtube.com/watch?v=lUqUbZnEXW4`
- **Duration:** 26 min
- **What You'll Build:** Security tests in Postman collections
- **Tools:** Postman, JavaScript
- **Hands-On:** Create test suite for API vulnerabilities

### 2.3 Container Scanning

**Video:** Trivy Image Scanning - Complete Tutorial
- **Source:** YouTube - AquaSecOfficial
- **Link:** `https://www.youtube.com/watch?v=oEX98i6vOUc`
- **Duration:** 28 min
- **What You'll Build:** Scan Docker images, identify vulnerabilities
- **Tools:** Trivy, Docker
- **Hands-On:** Scan public images, harden Dockerfile

**Video:** Trivy in GitHub Actions CI/CD
- **Source:** YouTube - AquaSecOfficial
- **Link:** `https://www.youtube.com/watch?v=5FwPiYNqZPU`
- **Duration:** 17 min
- **What You'll Build:** Automated image scanning on build
- **Tools:** Trivy, GitHub Actions
- **Hands-On:** Block push if vulnerabilities found

**Video:** Aqua Security ContainerD Scanning
- **Source:** YouTube - AquaSecOfficial
- **Link:** `https://www.youtube.com/watch?v=tKeY7uTvYxI`
- **Duration:** 21 min
- **What You'll Build:** Advanced container runtime scanning
- **Tools:** Aqua Security
- **Hands-On:** Monitor running containers for threats

**Video:** Harbor Registry with Image Scanning
- **Source:** YouTube - Harbor Project
- **Link:** `https://www.youtube.com/watch?v=dj0emKAb1b8`
- **Duration:** 24 min
- **What You'll Build:** Private Docker registry with vulnerability scanning
- **Tools:** Harbor, Docker
- **Hands-On:** Push image, auto-scan, quarantine unsafe

**Video:** DockerSlim for Secure Minimal Images
- **Source:** YouTube - Cloud Native
- **Link:** `https://www.youtube.com/watch?v=KZ_iHfnYWcI`
- **Duration:** 16 min
- **What You'll Build:** Reduce image size, reduce attack surface
- **Tools:** DockerSlim
- **Hands-On:** Slim existing image, rescan

### 2.4 Infrastructure as Code Security

**Video:** Terraform Basics + Security Best Practices
- **Source:** YouTube - Techwith Lucy
- **Link:** `https://www.youtube.com/watch?v=V4waklkBC02`
- **Duration:** 38 min
- **What You'll Build:** Write IaC with security defaults
- **Tools:** Terraform, AWS
- **Hands-On:** Create VPC, RDS, security groups securely

**Video:** Checkov - Terraform/CloudFormation Scanning
- **Source:** YouTube - BridgecrewOfficial
- **Link:** `https://www.youtube.com/watch?v=c1WbVdFRlMw`
- **Duration:** 20 min
- **What You'll Build:** Validate IaC before deployment
- **Tools:** Checkov
- **Hands-On:** Scan Terraform, fix misconfigurations

**Video:** tfsec - Lightweight Terraform Scanner
- **Source:** YouTube - aquasecurity
- **Link:** `https://www.youtube.com/watch?v=3xH5DgNbKGk`
- **Duration:** 15 min
- **What You'll Build:** Quick security checks for Terraform
- **Tools:** tfsec
- **Hands-On:** Scan file, interpret violations

**Video:** CloudFormation Security with cfn-lint
- **Source:** YouTube - AWS
- **Link:** `https://www.youtube.com/watch?v=h7cArOhJzaM`
- **Duration:** 18 min
- **What You'll Build:** Validate AWS CloudFormation templates
- **Tools:** cfn-lint
- **Hands-On:** Scan template, fix issues

**Video:** Kubernetes YAML Security Validation
- **Source:** YouTube - kubesec.io
- **Link:** `https://www.youtube.com/watch?v=yzUbqR6J4EY`
- **Duration:** 19 min
- **What You'll Build:** Validate K8s manifests
- **Tools:** kubesec, kubeval
- **Hands-On:** Score Kubernetes configs

### 2.5 CI/CD Pipeline Building (GitHub Actions)

**Video:** GitHub Actions Complete Hands-On Course
- **Source:** YouTube - TraversyMedia
- **Link:** `https://www.youtube.com/watch?v=R8_veQiYBjI`
- **Duration:** 60 min
- **What You'll Build:** Complete CI/CD workflow from scratch
- **Tools:** GitHub Actions, YAML
- **Hands-On:** Build, test, deploy with workflows

**Video:** GitHub Actions Security Best Practices
- **Source:** YouTube - GitHub
- **Link:** `https://www.youtube.com/watch?v=Kls_lAh_2S0`
- **Duration:** 26 min
- **What You'll Build:** Secure secrets, use OIDC, least privilege
- **Tools:** GitHub Actions, GitHub Secrets
- **Hands-On:** Replace PAT with OIDC, audit access

**Video:** Multi-Stage CI/CD with GitHub Actions
- **Source:** YouTube - Academind
- **Link:** `https://www.youtube.com/watch?v=SLpUKAGSXyU`
- **Duration:** 32 min
- **What You'll Build:** Separate stages: build, test, deploy
- **Tools:** GitHub Actions
- **Hands-On:** Create complex workflow with conditions

---

## ADVANCED LEVEL (6-12 months) {#advanced}

### 3.1 Jenkins CI/CD Setup

**Video:** Jenkins Installation & Configuration
- **Source:** YouTube - TechWorldwithNana
- **Link:** `https://www.youtube.com/watch?v=7KCS70sCoK0`
- **Duration:** 45 min
- **What You'll Build:** Install Jenkins, configure jobs
- **Tools:** Jenkins, Docker
- **Hands-On:** Create first pipeline job

**Video:** Jenkins Declarative Pipeline Security
- **Source:** YouTube - Jenkins Official
- **Link:** `https://www.youtube.com/watch?v=7s3C9f9nV2U`
- **Duration:** 38 min
- **What You'll Build:** Write Jenkinsfile with security stages
- **Tools:** Jenkins, Groovy
- **Hands-On:** Add SAST, DAST, container scanning stages

**Video:** Jenkins + SonarQube Integration
- **Source:** YouTube - KK JavaTutorials
- **Link:** `https://www.youtube.com/watch?v=KUnMA7fbKO4`
- **Duration:** 32 min
- **What You'll Build:** Automated code quality gates
- **Tools:** Jenkins, SonarQube
- **Hands-On:** Block builds on quality threshold

**Video:** Jenkins + Docker Build Pipeline
- **Source:** YouTube - Kodekloud
- **Link:** `https://www.youtube.com/watch?v=1IA8yq3FScA`
- **Duration:** 28 min
- **What You'll Build:** Build, scan, push Docker images
- **Tools:** Jenkins, Docker, DockerHub
- **Hands-On:** Automated Docker pipeline

**Video:** Jenkins Declarative Pipeline + Kubernetes Deploy
- **Source:** YouTube - TechWorldwithNana
- **Link:** `https://www.youtube.com/watch?v=DebvMle9FqU`
- **Duration:** 42 min
- **What You'll Build:** Deploy to K8s from Jenkins
- **Tools:** Jenkins, Kubernetes
- **Hands-On:** Pipeline deploys to cluster

### 3.2 GitLab CI/CD Advanced

**Video:** GitLab CI/CD Complete Guide with Docker
- **Source:** YouTube - That DevOps Guy
- **Link:** `https://www.youtube.com/watch?v=qKX2p6SUEOY`
- **Duration:** 55 min
- **What You'll Build:** Full pipeline: build, test, scan, deploy
- **Tools:** GitLab CI/CD, Docker
- **Hands-On:** Multi-stage pipeline with security gates

**Video:** GitLab Container Registry + Security Scanning
- **Source:** YouTube - GitLab
- **Link:** `https://www.youtube.com/watch?v=8jjQPxiKSA8`
- **Duration:** 22 min
- **What You'll Build:** Built-in SAST/DAST in GitLab
- **Tools:** GitLab, container-scanning
- **Hands-On:** Enable and configure scans

**Video:** GitLab SAST + Dependency Scanning
- **Source:** YouTube - GitLab Official
- **Link:** `https://www.youtube.com/watch?v=u-C1VeJDKxs`
- **Duration:** 24 min
- **What You'll Build:** Automated security scanning
- **Tools:** GitLab
- **Hands-On:** Configure multiple scanners

### 3.3 Kubernetes Security Hardening

**Video:** Kubernetes Security Context Deep Dive
- **Source:** YouTube - KodeKloud
- **Link:** `https://www.youtube.com/watch?v=ub3fZv8utzI`
- **Duration:** 34 min
- **What You'll Build:** Pod/container security contexts
- **Tools:** Kubernetes, YAML
- **Hands-On:** Create restricted pods

**Video:** Kubernetes Network Policies from Scratch
- **Source:** YouTube - NetworkChuck
- **Link:** `https://www.youtube.com/watch?v=8i-CHa_Pwms`
- **Duration:** 28 min
- **What You'll Build:** Restrict pod-to-pod traffic
- **Tools:** Kubernetes, Calico/Weave
- **Hands-On:** Create deny-all policy, allow specific paths

**Video:** Kubernetes RBAC Complete Implementation
- **Source:** YouTube - TechWorldwithNana
- **Link:** `https://www.youtube.com/watch?v=G3R24JSlGjY`
- **Duration:** 40 min
- **What You'll Build:** Role-based access control
- **Tools:** Kubernetes
- **Hands-On:** Create service account, roles, bindings

**Video:** Pod Security Policies (PSP) & Pod Security Standards
- **Source:** YouTube - Kubernetes Official
- **Link:** `https://www.youtube.com/watch?v=Qy9_uEVMG3Q`
- **Duration:** 32 min
- **What You'll Build:** Enforce security standards cluster-wide
- **Tools:** Kubernetes
- **Hands-On:** Implement restricted PSP

**Video:** Kubernetes Secrets Encryption at Rest
- **Source:** YouTube - TechWorldwithNana
- **Link:** `https://www.youtube.com/watch?v=DiBIWWP1v3o`
- **Duration:** 26 min
- **What You'll Build:** Encrypt etcd secrets
- **Tools:** Kubernetes, encryptionconfig
- **Hands-On:** Enable encryption, verify

**Video:** Kubernetes Audit Logging Setup
- **Source:** YouTube - Kubernetes Official
- **Link:** `https://www.youtube.com/watch?v=Ds25VvWHsKc`
- **Duration:** 25 min
- **What You'll Build:** Log all API requests
- **Tools:** Kubernetes
- **Hands-On:** Configure audit policy, collect logs

### 3.4 Cloud Security (AWS Deep Dive)

**Video:** AWS Security Best Practices - VPC Security
- **Source:** YouTube - CloudAcademy
- **Link:** `https://www.youtube.com/watch?v=u7WnnZHTg1s`
- **Duration:** 48 min
- **What You'll Build:** Multi-tier VPC with security groups
- **Tools:** AWS, Terraform
- **Hands-On:** Create secure network architecture

**Video:** AWS EC2 Hardening Complete Guide
- **Source:** YouTube - CloudGuru
- **Link:** `https://www.youtube.com/watch?v=YB-NPa0KaFQ`
- **Duration:** 42 min
- **What You'll Build:** Secure EC2 instances
- **Tools:** AWS EC2, Systems Manager
- **Hands-On:** Patch, harden, monitor

**Video:** AWS S3 Security & Access Control
- **Source:** YouTube - TechWorldwithNana
- **Link:** `https://www.youtube.com/watch?v=4K7rvQqQ5oQ`
- **Duration:** 36 min
- **What You'll Build:** Private S3, encryption, versioning
- **Tools:** AWS S3
- **Hands-On:** Configure bucket policies, CORS

**Video:** AWS IAM Least Privilege Setup
- **Source:** YouTube - CloudMaven
- **Link:** `https://www.youtube.com/watch?v=qBMoLW6yU8I`
- **Duration:** 38 min
- **What You'll Build:** Create restricted IAM roles/policies
- **Tools:** AWS IAM
- **Hands-On:** Create custom policy, test permissions

**Video:** AWS CloudTrail Logging & Monitoring
- **Source:** YouTube - AWS
- **Link:** `https://www.youtube.com/watch?v=KXH-HFDTfDw`
- **Duration:** 32 min
- **What You'll Build:** Audit trail setup, analysis
- **Tools:** AWS CloudTrail, CloudWatch
- **Hands-On:** Query logs for suspicious activity

**Video:** AWS WAF (Web Application Firewall) Setup
- **Source:** YouTube - Pluralsight
- **Link:** `https://www.youtube.com/watch?v=BV8eR0vAK9M`
- **Duration:** 28 min
- **What You'll Build:** Protect ALB/CloudFront from attacks
- **Tools:** AWS WAF
- **Hands-On:** Create rules, test blocking

**Video:** AWS Secrets Manager for Application Secrets
- **Source:** YouTube - Tutorials Dojo
- **Link:** `https://www.youtube.com/watch?v=S_rNVlXLJoE`
- **Duration:** 24 min
- **What You'll Build:** Rotate secrets, integrate apps
- **Tools:** AWS Secrets Manager, Lambda
- **Hands-On:** Store secret, retrieve from app

### 3.5 Cloud Security (Azure Deep Dive)

**Video:** Azure Security Best Practices - Network Setup
- **Source:** YouTube - CloudAcademy
- **Link:** `https://www.youtube.com/watch?v=jXY4cZZ3xEE`
- **Duration:** 46 min
- **What You'll Build:** Secure Azure VNet, NSG rules
- **Tools:** Azure, Terraform
- **Hands-On:** Create multi-tier network

**Video:** Azure App Service Security Hardening
- **Source:** YouTube - John Hammond
- **Link:** `https://www.youtube.com/watch?v=E8_F_5gAKS0`
- **Duration:** 35 min
- **What You'll Build:** Secure web app deployment
- **Tools:** Azure App Service
- **Hands-On:** Enable authentication, SSL, firewalls

**Video:** Azure SQL Database Security (Encryption, Audit, Threat Detection)
- **Source:** YouTube - Microsoft Learn
- **Link:** `https://www.youtube.com/watch?v=7gx5H4oD_LQ`
- **Duration:** 40 min
- **What You'll Build:** Secure database deployment
- **Tools:** Azure SQL Database
- **Hands-On:** Enable encryption, auditing

**Video:** Azure Key Vault Managed Identity Integration
- **Source:** YouTube - John Hammond
- **Link:** `https://www.youtube.com/watch?v=kQHuOj0nS5w`
- **Duration:** 32 min
- **What You'll Build:** Apps authenticate without credentials
- **Tools:** Key Vault, Managed Identity
- **Hands-On:** App retrieves secrets securely

**Video:** Azure DevSecOps with Azure DevOps & Pipelines
- **Source:** YouTube - Microsoft
- **Link:** `https://www.youtube.com/watch?v=_N-5M9nXa_M`
- **Duration:** 48 min
- **What You'll Build:** Full DevSecOps pipeline
- **Tools:** Azure DevOps, Pipelines
- **Hands-On:** Build, test, scan, deploy

**Video:** Azure Defender for Cloud Security
- **Source:** YouTube - Microsoft Learn
- **Link:** `https://www.youtube.com/watch?v=cFZJIwLc5VU`
- **Duration:** 35 min
- **What You'll Build:** Continuous security monitoring
- **Tools:** Azure Defender
- **Hands-On:** Enable recommendations, remediate

### 3.6 Cloud Security (GCP Deep Dive)

**Video:** GCP Security Best Practices VPC & Firewall
- **Source:** YouTube - CloudAcademy
- **Link:** `https://www.youtube.com/watch?v=YdhU1x5uGlo`
- **Duration:** 42 min
- **What You'll Build:** Secure GCP network
- **Tools:** GCP, gcloud CLI
- **Hands-On:** Create VPC, firewall rules

**Video:** GCP Cloud Run Security Hardening
- **Source:** YouTube - Google Cloud
- **Link:** `https://www.youtube.com/watch?v=jS_iSJEb_3o`
- **Duration:** 28 min
- **What You'll Build:** Deploy containerized apps securely
- **Tools:** Cloud Run, Container Registry
- **Hands-On:** Deploy, configure security

**Video:** GCP Cloud SQL Encryption & Authentication
- **Source:** YouTube - Google Cloud
- **Link:** `https://www.youtube.com/watch?v=WMFp5Iix_uc`
- **Duration:** 30 min
- **What You'll Build:** Secure database
- **Tools:** Cloud SQL
- **Hands-On:** Enable encryption, SSL, IAM

**Video:** GCP IAM Deep Dive - Custom Roles
- **Source:** YouTube - CloudAcademy
- **Link:** `https://www.youtube.com/watch?v=qeY8JiIAqOE`
- **Duration:** 36 min
- **What You'll Build:** Fine-grained access control
- **Tools:** GCP IAM
- **Hands-On:** Create custom roles

**Video:** GCP Cloud Armor DDoS Protection
- **Source:** YouTube - Google Cloud
- **Link:** `https://www.youtube.com/watch?v=q8GmVsOFWUM`
- **Duration:** 22 min
- **What You'll Build:** WAF with Cloud Armor
- **Tools:** Cloud Armor, Load Balancer
- **Hands-On:** Create rules, test protection

### 3.7 Cloud Security (OCI Deep Dive)

**Video:** OCI VCN (Virtual Cloud Network) Security Setup
- **Source:** YouTube - Oracle University
- **Link:** `https://www.youtube.com/watch?v=3RW2PVpQCoI`
- **Duration:** 38 min
- **What You'll Build:** Secure OCI network
- **Tools:** OCI VCN, Security Lists
- **Hands-On:** Create isolated network

**Video:** OCI Compute (VM) Hardening & Monitoring
- **Source:** YouTube - Oracle Cloud
- **Link:** `https://www.youtube.com/watch?v=dX5xJScuT0Y`
- **Duration:** 35 min
- **What You'll Build:** Secure instance deployment
- **Tools:** OCI Compute
- **Hands-On:** Configure OS hardening

**Video:** OCI Database Security (Encryption, Audit, TDE)
- **Source:** YouTube - Oracle University
- **Link:** `https://www.youtube.com/watch?v=ZwqrXjzN2Og`
- **Duration:** 40 min
- **What You'll Build:** Enterprise database security
- **Tools:** OCI Database
- **Hands-On:** Enable all security features

