# CI/CD with GitHub Actions + Amazon ECS
This repository has two ways to store the spring boot application image, you can check the code under `.github/workflows`

## 1. Using Docker Hub 
Create an access token to authorize the runner to use your docker hub account: https://app.docker.com/settings/personal-access-tokens  

Add variables:
- AWS_REGION
- DOCKER_IMAGE_NAME
- DOCKER_USERNAME
- ECS_CLUSTER_NAME
- ECS_CONTAINER_NAME
- ECS_SERVICE_NAME
- ECS_TASK_DEFINITION_FAMILY_NAME

Add secrets:
- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY
- DOCKER_ACCESS_TOKEN

## Using ECR private repository

Add variables:
- AWS_REGION
- ECR_REPOSITORY_NAME
- ECS_CLUSTER_NAME
- ECS_CONTAINER_NAME
- ECS_SERVICE_NAME
- ECS_TASK_DEFINITION_FAMILY_NAME

Add secrets:
- AWS_ACCESS_KEY_ID
- AWS_SECRET_ACCESS_KEY
