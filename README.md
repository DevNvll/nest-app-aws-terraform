# Dockerized App Terraform boilerplate for AWS

Simplest boilerplate for a NestJS app (or any other dockerized app) Terraform config for AWS deployment.

## What it does

It creates an ECS Cluster, ECS Service, ECS Task Definition (and it's security groups), Load Balancer (and its target groups) and ECR repository. It follows this naming convention "%app_name%-cluster", "%app_name%-service", "%app_name%-task", "%app_name%-lb".

`app_name` variable will be prompted upon `terraform plan` or `terraform apply`

It uses your AWS account default VPC and subnets.
