# 🚀 Terraform Docker Container Provisioning

This repository contains Terraform code to provision a local Docker container (Nginx) using Infrastructure as Code (IaC).

---

## 📝 Overview

This project demonstrates how to use Terraform with the Docker provider to automate the creation and management of a local Docker container. The container runs the latest Nginx image and maps port 8050 on the host to port 80 in the container.

---

## 📁 Project Structure

```
terraform-docker/
  ├── main.tf
  ├── README.md
```

## ⚙️ Prerequisites

- [Terraform](https://developer.hashicorp.com/terraform/downloads) installed
- [Docker](https://www.docker.com/products/docker-desktop) installed and running locally
- Basic knowledge of command-line interface (CLI) and Git

---

## 🚀 Setup & Usage

**1. Clone the repository**

   ```
   git clone https://github.com/Utkarsh067/terraform-docker.git
   cd terraform-docker
   ```

**2. Initialize Terraform**

  ```terraform init```

**3. Review planned changes**

  ```terraform plan```

**4. Apply the configuration**

  ```terraform apply```

Type ```yes``` when prompted.

**5. Verify the container is running**

Open your browser and go to ```http://localhost:8050``` — you should see the Nginx welcome page.

![Screenshot 2025-05-30 144413](https://github.com/user-attachments/assets/24fda1d7-7e2b-48b8-9d12-d96eaaa670c4)

Or check via Docker CLI:

```docker ps```

## 🧹 Cleaning Up

To destroy the Docker container and clean up resources created by Terraform:

```terraform destroy```

Type ```yes``` to confirm.

## 💡 Notes

+ The container runs Nginx, but you can modify main.tf to use any other Docker image.

+ Ports can be customized by changing the ports block in main.tf.

# ✍️ Author

Utkarsh Jain

[LinkedIn](https://www.linkedin.com/in/utkarsh-jain02/)
