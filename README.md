# US-Visa-Approval-Prediction

## Live matarials docs

[link](https://docs.google.com/document/d/1UFiHnyKRqgx8Lodsvdzu58LbVjdWHNf-uab2WmhE0A4/edit?usp=sharing)


## Git commands

```bash
git add .

git commit -m "Updated"

git push origin main
```

## How to run?

```bash
conda create -n visa python=3.8 -y
```

```bash
conda activate visa
```

```bash
pip install -r requirements.txt
```

```bash
python app.py
```


## Workflow

1. constant
2. config_entity
3. artifact_entity
4. conponent
5. pipeline
6. app.py / demo.py


### Export the  environment variable
```bash


export MONGODB_URL="mongodb+srv://<username>:<password>...."

export AWS_ACCESS_KEY_ID=<AWS_ACCESS_KEY_ID>

export AWS_SECRET_ACCESS_KEY=<AWS_SECRET_ACCESS_KEY>
```



# AWS-CICD-Deployment-with-Github-Actions

## 1. Login to AWS console.

## 2. Create IAM user for deployment

	#with specific access

	1. EC2 access : It is virtual machine

	2. ECR: Elastic Container registry to save your docker image in aws


	#Description: About the deployment

	1. Build docker image of the source code

	2. Push your docker image to ECR

	3. Launch Your EC2 

	4. Pull Your image from ECR in EC2

	5. Lauch your docker image in EC2

	#Policy:

	1. AmazonEC2ContainerRegistryFullAccess

	2. AmazonEC2FullAccess

	
## 3. Create ECR repo to store/save docker image
    - Save the URI: 136566696263.dkr.ecr.us-east-1.amazonaws.com/mlproject

	
## 4. Create EC2 machine (Ubuntu) 

## 5. Open EC2 and Install docker in EC2 Machine:
	
	
	#optinal

	sudo apt-get update -y

	sudo apt-get upgrade
	
	#required

	curl -fsSL https://get.docker.com -o get-docker.sh

	sudo sh get-docker.sh

	sudo usermod -aG docker ubuntu

	newgrp docker
	
# 6. Configure EC2 as self-hosted runner:
    setting>actions>runner>new self hosted runner> choose os> then run command one by one


# 7. Setup github secrets:

   - AWS_ACCESS_KEY_ID
   - AWS_SECRET_ACCESS_KEY
   - AWS_DEFAULT_REGION
   - ECR_REPO

    
# Folder Structure
![1_Folder Structure](https://github.com/AveshVerma/Visa-Approval-Prediction-Project-in-Production/assets/100403248/e08faee0-40f0-49fc-8971-2698a3077835)

# Data Ingestion
![Data Ingestion](https://github.com/AveshVerma/Visa-Approval-Prediction-Project-in-Production/assets/100403248/92d8a19d-37b1-481e-bb8d-11680d253e0c)

# Data Transformation
![Data Transformation](https://github.com/AveshVerma/Visa-Approval-Prediction-Project-in-Production/assets/100403248/b6d6c689-cd41-489b-80da-131ec5badad2)

# Data Validation
![Data Validation](https://github.com/AveshVerma/Visa-Approval-Prediction-Project-in-Production/assets/100403248/8e7c8069-a267-4546-896f-f516e21dd061)

# Model Trainer
![Model Trainer](https://github.com/AveshVerma/Visa-Approval-Prediction-Project-in-Production/assets/100403248/2acd5f5d-8dda-41b3-9074-21040f0d8a75)

# Model Evaluation
![Model Evaluation](https://github.com/AveshVerma/Visa-Approval-Prediction-Project-in-Production/assets/100403248/0448c9f8-8564-4596-9753-251f3f60d093)

# Model Pusher
![Model Pusher](https://github.com/AveshVerma/Visa-Approval-Prediction-Project-in-Production/assets/100403248/1158ffa1-234a-4a19-92e6-cb9ff59ced7e)

