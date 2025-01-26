🚀 Project Overview
This project demonstrates the deployment and management of a scalable, secure, and highly available infrastructure on AWS using Terraform. By adopting Infrastructure as Code (IaC) principles, the project highlights efficient and robust cloud architecture design and implementation.

The infrastructure features a Virtual Private Cloud (VPC) with public subnets, an internet gateway, and custom route tables to facilitate efficient and secure network communication. EC2 instances were provisioned with custom user data scripts to host web applications using the Apache web server, ensuring automated server setup and consistent deployments. An Application Load Balancer (ALB) was configured to distribute traffic across multiple EC2 instances, achieving redundancy and fault tolerance. Additionally, reusable Terraform modules were developed to streamline the provisioning of key AWS resources, including S3 buckets for object storage, ALB configurations for traffic management, and security groups with precise ingress and egress rules.

To enhance performance and reliability, target groups were created and attached to the ALB for application health monitoring and traffic optimization. Furthermore, AWS CLI commands were integrated within user data scripts to dynamically retrieve instance metadata, enabling more adaptive and functional server configurations.

🛠️ Technologies Used
This project leverages Terraform for cloud infrastructure automation and key AWS services such as EC2, VPC, subnets, ALB, S3, and security groups. Bash scripting was utilized for server setup automation, while the Apache web server was used to host and serve web applications efficiently.

📋 Steps to Configure
To deploy the infrastructure, begin by initializing Terraform in the project directory to download the necessary provider plugins using the terraform init command. Once initialized, validate the configuration files for errors or missing dependencies by running terraform validate. After ensuring everything is in order, apply the Terraform plan with terraform apply to provision the AWS resources. When the infrastructure is no longer needed, clean up resources using terraform destroy, which will tear down all deployed components.

