# end_to_end_ml_project

# Deployed end to end project in aws ec2 via github

1. create .yaml file. Required it should be inside <./github/workflows>

# Create ECR container registry in AWS Console
# 008971679870.dkr.ecr.us-east-1.amazonaws.com/my-common-repo

# Create EC2 instance 

# Connect to instance

# Steps to follow after connecting instance
sudo apt update 

apt list --upgradable

# If above commands doesn't work, then try this
sudo apt-get update -y

sudo apt get upgrade

# Commands to install Docker in EC2

curl -fsSL https://get.docker.com -o get-docker.sh

sudo sh get-docker.sh

sudo usermod -aG docker ubuntu

newgrp docker

verify - docker --verion


# Github settings
1. go to working repository
2. go to settings -> actions -> runners -> create self-hosted runner
3. follow the commnads provided in Running EC2 instance
4. go to settings -> secrets and variable -> add secrets

# AWS_ACCESS_KEY_ID
# AWS_SECRET_ACCESS_KEY
# AWS_REGION
# AWS_ECR_LOGIN_URI
# ECR_REPOSITORY_NAME