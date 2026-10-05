# DevOps Internship Task 3 – Infrastructure as Code with Terraform

## Objective

Provision a local Docker container using Terraform as Infrastructure as Code (IaC).

## Tools Used

* Terraform
* Docker Desktop
* Nginx
* VS Code

## Project Description

In this task, Terraform was used to provision and manage a Docker-based Nginx container locally.

Terraform created the Nginx Docker image and a Docker container named `terraform-nginx`.

## Resources Created

* Docker Image: `nginx:latest`
* Docker Container: `terraform-nginx`
* Port Mapping: `8080:80`

## Terraform Commands Used

```bash
terraform init
terraform plan
terraform apply
terraform state list
terraform destroy
```

## Verification

The running container was verified using:

```bash
docker ps
```

The Nginx application was accessed through:

```text
http://localhost:8080
```

The Nginx Welcome page was displayed successfully.

Terraform-managed resources were verified using:

```bash
terraform state list
```

Resources:

```text
docker_image.nginx
docker_container.nginx
```

## Cleanup

After successful verification, all Terraform-managed resources were removed using:

```bash
terraform destroy
```

The destroy operation completed successfully with 2 resources destroyed.

## Outcome

This task provided practical experience with Infrastructure as Code (IaC) using Terraform and demonstrated how to provision, manage, verify, and destroy Docker infrastructure locally.
