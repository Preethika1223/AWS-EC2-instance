# AWS-EC2-instance
# EC2 Instance Setup Guide

This guide provides step-by-step instructions to launch an EC2 instance in AWS. Follow the steps carefully to ensure the instance is configured correctly.

---

## Prerequisites
- An active AWS account.
- Access to the AWS Management Console.
- A key pair (create Key pair) and save the .pem file for future reference
---

## Steps to Launch an EC2 Instance

1. **Log in to AWS Console**
   - Go to the [AWS Management Console](https://aws.amazon.com/console/).
   - Log in with your credentials.

2. **Select the Region**
   - On the top-right corner of the console, ensure the region is set :For example
     - **us-east-1 (N. Virginia)** ,
     - **us-west-2 (Oregon)**.

3. **Navigate to EC2**
   - In the AWS Management Console, search for **EC2** in the services menu and click on it.

4. **Launch an Instance**
   - Click on the **Launch Instance** button.

5. **Name Your Instance**
   - Provide a name for your instance in the following format:
     ```
     name_EC2
     ```
   - **Note:** Unnamed instances will be terminated.

6. **Choose an Amazon Machine Image (AMI)**(cheaper)
   - Select **Amazon Linux**.
   - Choose **Amazon Linux 2023 AMI**.

7. **Select Instance Type**
   - Choose either **t2.micro** or **t3.micro**.
   - **Important:** Do not select any other instance type.

8. **Key Pair**
   - Under **Key pair (login)**, click on the dropdown and select **Key pair which we created**.

9. **Network Settings**
   - Under **Firewall (security groups)**, select **Create security group**.
   - Configure the security group as needed (e.g., allow SSH access from your IP).

10. **Launch the Instance**
    - Review all the settings to ensure they are correct.
    - Click **Launch Instance**.

11. **Verify the Instance**
    - Go to the EC2 Dashboard and check if your instance is running.
    - Ensure the instance name follows the required naming convention.

---

## Notes
- Use only **t2.micro** or **t3.micro** instance types to avoid unnecessary costs.
- Unnamed instances or instances with incorrect configurations will be terminated.

---

## Troubleshooting
- If you encounter issues, verify the following:
  - region is selected.
  - Key pair is available.
  - Instance type is either **t2.micro** or **t3.micro**.

---



