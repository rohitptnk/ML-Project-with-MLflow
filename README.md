# ML-Project-with-MLflow

## Workflows

1. Update config.yaml
2. Update schema.yaml
3. Update params.yaml
4. Update the entity
5. Update the configuaration manager in src config
6. Update the components
7. Update the pipeline
8. Update the main.py
9. Update the app.py


AWS URI: 149999905817.dkr.ecr.ap-southeast-2.amazonaws.com/mlflowproj

## Install docker in EC2 Machine
```
sudo apt-get update -y
sudo apt-get upgrade
curl -fsSL https://get.docker.com -o get-docker.sh
sudo sh get-docker.sh
sudo usermod -aG docker ubuntu
newgrp docker

```

## Configure EC2 as self hosted runner
setting>actions>runner>new self hosted runner> choose os> then run command one by one
name of the runner group: Enter
name of the runner: self-hosted
Enter, Enter

# Setup Github secrets
AWS_ACCESS_KEY_ID= (from the csv)
AWS_SECRET_ACCESS_KEY= (from the csv)
AWS_REGION=ap-southeast-2 (the region)
AWS_ECR_LOGIN_URI=149999905817.dkr.ecr.ap-southeast-2.amazonaws.com
ECR_REPOSITORY_NAME=mlflowproj