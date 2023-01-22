## Infrastructure
This folder contains Terraform configurations files that will:
1. Create an ECR repo for the docker image
2. Create an ECS Cluster, Service and Fargate task definition which will use the container
3. Create a Load Balancer, security group, target group and listener
4. Set up Autoscaling for the Fargate tasks based on CPU Utilization and Memory Utilization metrics

Please note that once the ECR repo is created, you will need to build a docker image and push it to the repo before creating the service.