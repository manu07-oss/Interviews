# Navi Interview Preparation Notes

## 🧠 Topics Covered in Interview

### 1. CI/CD Pipeline (GitLab)

* Code flow: feature → merge request → main branch
* CI stages:

  * Code scan (Semgrep, SonarQube)
  * Build
  * Artifact (JFrog)
  * Security scan (Trivy)
* CD stages:

  * Push to ECR
  * Deploy to ECS/EKS

---

### 2. Kubernetes (Weak Area ⚠️)

* Deployment strategy (Rolling update)
* Control Plane components
* Worker Node components
* OOMKilled
* CrashLoopBackOff
* Helm basics
* Deployment vs StatefulSet

---

### 3. AWS Core Concepts

* VPC, Subnets
* Route Tables
* Internet Gateway vs NAT Gateway
* Security Group vs NACL
* VPC Peering vs Transit Gateway
* IAM policies

---

### 4. Terraform

* State file
* Backend (S3)
* State remove
* Modules

---

### 5. Linux & CLI

* SSH / SCP
* Basic commands

---

## 🔴 Weak Areas Identified

* Kubernetes depth
* AWS networking fundamentals
* CLI commands

---

## ✅ Key Interview Answers

### Kubernetes Deployment Strategy

* Default: Rolling Update
* Gradually replaces old pods with new ones

---

### Kubernetes Control Plane

* API Server → Entry point
* etcd → Stores cluster state
* Scheduler → Assigns pods
* Controller Manager → Maintains state

---

### Worker Node Components

* kubelet → Manages pods
* kube-proxy → Networking
* Container runtime → Runs containers

---

### OOMKilled

* Container exceeded memory limit

---

### CrashLoopBackOff

* Container repeatedly failing

---

### Helm

* Kubernetes package manager
* Used to deploy applications via charts

---

### AWS Subnets

* Public → Internet Gateway
* Private → NAT Gateway

---

### Route Table

* Public: 0.0.0.0/0 → Internet Gateway
* Private: 0.0.0.0/0 → NAT Gateway

---

### Internet Gateway vs NAT Gateway

* IGW → inbound + outbound
* NAT → outbound only

---

### Security Group vs NACL

* SG → Instance level, Stateful
* NACL → Subnet level, Stateless

---

### VPC Peering

* Connects two VPCs directly (low cost)

---

### Terraform State Remove

```bash
terraform state rm <resource_name>
```

---

### AWS CLI Examples

```bash
aws s3 ls
aws s3 ls s3://bucket-name
```

---

### SSH Command

```bash
ssh -i key.pem ec2-user@ip-address
```

---

## 📚 Learning Resources

### Kubernetes

* [https://kubernetes.io/docs/home/](https://kubernetes.io/docs/home/)
* TechWorld with Nana (YouTube)

### AWS

* [https://docs.aws.amazon.com/](https://docs.aws.amazon.com/)
* freeCodeCamp AWS course

### Terraform

* [https://developer.hashicorp.com/terraform/docs](https://developer.hashicorp.com/terraform/docs)

### Linux

* [https://linuxjourney.com/](https://linuxjourney.com/)

### DevOps Roadmap

* [https://roadmap.sh/devops](https://roadmap.sh/devops)

---

## 🚀 Action Plan

### Week 1

* Kubernetes basics
* kubectl practice

### Week 2

* AWS networking deep dive
* IAM + S3 + EC2

### Week 3

* Terraform hands-on
* CI/CD explanation practice

---

## 💬 Notes

* Strength: Real project experience
* Improve: Fundamentals + Kubernetes + confidence
