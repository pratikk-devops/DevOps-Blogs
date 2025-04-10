
# AWS EC2 and Security Groups Setup Guide

This guide walks you through creating and configuring **AWS Security Groups** for your EC2 instance.

## Prerequisites
- An **AWS** account (free-tier works fine).
- Basic knowledge of AWS EC2 and security.

---

## Step 1: Login to AWS Management Console
1. Go to the [AWS Management Console](https://aws.amazon.com/).
2. Sign in or create a new account.

## Step 2: Navigate to EC2 Dashboard
1. In the search bar, type **EC2** and select **EC2 Dashboard**.

## Step 3: Create a New Security Group
1. On the left, under **Network & Security**, click **Security Groups**.
2. Click **Create Security Group**.
3. Enter:
   - **Security Group Name**: e.g., "MyWebServerSG".
   - **Description**: e.g., "Security Group for my EC2 instance".
   - **VPC**: Choose the default VPC.

## Step 4: Add Inbound Rules
1. Click **Inbound Rules**.
2. Click **Add Rule**:
   - **SSH** (port 22) for Linux/Unix instances.
   - **HTTP** (port 80) for web servers.
   - **HTTPS** (port 443) for secure websites.
3. Set the **Source** to **0.0.0.0/0** for global access or restrict to specific IPs for more security.

## Step 5: Add Outbound Rules
1. By default, outbound traffic is allowed (0.0.0.0/0).
2. You can modify this for tighter security if needed.

## Step 6: Review and Create Security Group
1. Review your settings and click **Create Security Group**.

## Step 7: Associate Security Group with EC2 Instance
1. Go to **Instances** in the EC2 Dashboard.
2. Select your instance and click **Actions > Networking > Change Security Groups**.
3. Select the newly created Security Group and click **Apply**.

---

## Tips for EC2 Security:
- **Limit SSH Access**: Restrict access to specific IPs (avoid 0.0.0.0/0).
- **Use SSH Key Pairs**: For secure login, use key pairs instead of passwords.
- **Least Privilege**: Only open necessary ports and restrict access.

---

**Congrats!** You’ve successfully configured your EC2 instance’s security group. Keep exploring AWS and improving your cloud security skills! 🌐🚀

#aws #ec2 #securitygroups #cloudcomputing #devops #learninginpublic #techbeginner #cloudsecurity
