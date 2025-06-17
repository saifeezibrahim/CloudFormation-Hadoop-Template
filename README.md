# 🏗️ AWS CloudFormation Hadoop Cluster Template (3-Node) — Learning Lab

> **A hands-on, beginner-friendly project to deploy your own Hadoop cluster on AWS using CloudFormation. Perfect for DevOps & Big Data learners!**

---

## 🚀 What is This Project?

This repo gives you a ready-to-use AWS CloudFormation template and helper scripts to spin up a **3-node Hadoop cluster** on EC2.  
It's designed for:
- Learning AWS CloudFormation in a practical, real-world context
- Experimenting with Hadoop clusters without manual setup
- Building your DevOps and Big Data deployment skills

---

## 📦 What's Included?

```plaintext
README.md        # This guide!
template.yaml    # CloudFormation template for the Hadoop cluster (edit, study, reuse)
launch.sh        # Helper script to launch your stack with environment variables
LICENSE          # License info
```
👉 [Explore all files in GitHub](https://github.com/saifeezibrahim/CloudFormation-Hadoop-Template/tree/master)

---

## 🛠️ Prerequisites

- AWS account (with CloudFormation, EC2, and VPC permissions)
- AWS CLI installed and configured (`aws configure`)
- An existing VPC (see [AWS VPC Guide](https://docs.aws.amazon.com/directoryservice/latest/admin-guide/gsg_create_vpc.htm))
- An AWS EC2 SSH Key Pair

---

## 🚦 Quick Start Guide

### 1. **Clone & Prepare**
```bash
git clone https://github.com/saifeezibrahim/CloudFormation-Hadoop-Template.git
cd CloudFormation-Hadoop-Template
```

### 2. **Set Environment Variables**
```bash
export STACK_NAME='your-stack-name'
export SSH_KEY_NAME='your-aws-key-name'
export VPC_CIDR='your-vpc-cidr'  # e.g. 172.31.0.0/16
```

### 3. **Launch the Cluster!**
- **Easy mode:**  
  ```bash
  ./launch.sh
  ```
  This will use the defaults and your environment variables.

- **Customize:**  
  Edit `template.yaml` or invoke your own `aws cloudformation create-stack` command for more control.

### 4. **Monitor Progress**
- Watch your stack in the AWS Console → CloudFormation.

### 5. **Connect & Explore**
- After stack creation, SSH into your Hadoop nodes using your keypair and public IPs.
- Experiment with Hadoop, cluster networking, or CloudFormation edits!

### 6. **Delete Your Stack**
- **Command line:**
  ```bash
  aws cloudformation delete-stack --stack-name ${STACK_NAME}
  ```
- **AWS Console:**  
  Go to CloudFormation and delete the stack.

---

## 🎓 Learning Outcomes

- Understand how to automate infrastructure with CloudFormation
- See real-world VPC, EC2, and Security Group setup
- Practice launching and managing Hadoop clusters in the cloud
- Safely experiment with stack updates and deletions

---

## 💡 Pro Tips

- Break, edit, and fix the template to maximize your learning!
- Try scaling node count or customizing instance types.
- Explore adding bootstrap actions or configuring Hadoop further.

---

## 🙋‍♂️ Credits

Maintained by **Saifee Ibrahim**  
Fork, star and share if you find this useful for your learning journey!

---

## 📄 License

MIT — Free for learning and educational use.

---

> **Start building, breaking and learning — real cloud skills come from doing!**
