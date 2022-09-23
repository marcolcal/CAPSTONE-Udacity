# CAPSTONE-Udacity
##Capstone Project for the Udacity NanoDegree

The main purpose of the project is to demostrate the skills and knowledge gained thoughtout the course Cloud Devops Nanodegree. The course covered all source of techniques for Cloud Devops Engineers to work with AWS resources to create a CICD process to deplou, configure and provision infrastructure. 

#Scope of work:
You will develop a CI/CD pipeline for micro services applications with either blue/green deployment or rolling deployment. You will also develop your Continuous Integration steps as you see fit, but must at least include typographical checking (aka “linting”). To make your project stand out, you may also choose to implement other checks such as security scanning, performance testing, integration testing, etc.!

Once you have completed your Continuous Integration you will set up Continuous Deployment, which will include:

Pushing the built Docker container(s) to the Docker repository (you can use AWS ECR, create your own custom Registry within your cluster, or another 3rd party Docker repository) ; and
Deploying these Docker container(s) to a small Kubernetes cluster. For your Kubernetes cluster you can either use AWS Kubernetes as a Service, or build your own Kubernetes cluster. To deploy your Kubernetes cluster, use either Ansible or Cloudformation. Preferably, run these from within Jenkins or Circle CI as an independent pipeline.

#Specifications:
##PROJECT SPECIFICATION
###Capstone- Cloud DevOps
  - Create Github repository with project code.
  - Set Up Pipeline
  - Use image repository to store Docker images (Docker Hub)
  - Build Docker Container
  - Execute linting step in code pipeline
  - Code is checked against a linter as part of a Continuous Integration step (demonstrated w/ two screenshots)
  - Build a Docker container in a pipeline
  - The project takes a Dockerfile and creates a Docker container in the pipeline.
  - Successful Deployment
  - The Docker container is deployed to a Kubernetes cluster
  - The cluster is deployed with CloudFormation or Ansible. This should be in the source code of the student’s submission.
  - Use Blue/Green Deployment or a Rolling Deployment successfully 
  - The project performs the correct steps to do a blue/green or a rolling deployment into the environment selected. 
    Student demonstrates the successful completion of  chosen deployment methodology with screenshots.



##Tools and Processes
### CI/CD Tools and Cloud Services

* [Circle CI](https://www.circleci.com) - Cloud-based CI/CD service
* [Amazon AWS](https://aws.amazon.com/) - Cloud services
* [AWS EKS](https://aws.amazon.com/eks/) - Amazon Elastic Kubernetes Services
* [AWS eksctl](https://eksctl.io) - The official CLI for Amazon EKS
* [AWS CLI](https://aws.amazon.com/cli/) - Command-line tool for AWS
* [kubectl](https://kubernetes.io/docs/reference/kubectl/) - a command-line tool to control Kubernetes clusters
* [Docker Hub](https://hub.docker.com/repository/docker/ovolmar/flask-blue) - Container images repository service

#### CicleCI Variables
| VARIABLE | VALUE |
| ------ | ------ |
| AMI | _redacted_** |
| ARN | arn:partition:service:region:account-id:resource-id |
| AWS_ACCESS_KEY_ID | _redacted_** |
| AWS_DEFAULT_REGION | _redacted_** |
| AWS_SECRET_ACCESS_KEY | _redacted_** |
| DOCKER_LOGIN | _redacted_** |
| DOCKER_TOKEN| _redacted_** |
| IMAGE_NAME | Docker image name |
|REGISTRY_URL | Your docker registry |
| AWS_PEM_KEY | _redacted_** |


#Step to Complete.
##Steps in Completing Your Project
* Step 1: Propose and Scope the Project
  Plan what your pipeline will look like.
  Decide which options you will include in your Continuous Integration phase. Use either Circle CI or Jenkins.
  Pick a deployment type - either rolling deployment or blue/green deployment.
  For the Docker application you can either use an application which you come up with, or use an open-source application pulled from the Internet, or if you have no     idea, you can use an Nginx “Hello World, my name is (student name)” application.
* Step 2: Use Jenkins or Circle CI, and implement blue/green or rolling deployment.
  If you're using Jenkins, create your Jenkins master box and install the plugins you will need.
  If you're using Circle CI, set up your circle CI account and connect your git repository.
  Set up your environment to which you will deploy code.
* Step 3: Pick AWS Kubernetes as a Service, or build your own Kubernetes cluster.
  Use Ansible or CloudFormation to build your “infrastructure”; i.e., the Kubernetes Cluster.
  It should create the EC2 instances (if you are building your own), set the correct networking settings, and deploy software to these instances.
  As a final step, the Kubernetes cluster will need to be initialized. The Kubernetes cluster initialization can either be done by hand, or with Ansible/Cloudformation   at the student’s discretion.
* Step 4: Build your pipeline
  Construct your pipeline in your GitHub repository.
  Set up all the steps that your pipeline will include.
  Configure a deployment pipeline.
  Include your Dockerfile/source code in the Git repository.
  Include with your Linting step both a failed Linting screenshot and a successful Linting screenshot to show the Linter working properly.
* Step 5: Test your pipeline
  Perform builds on your pipeline.
  Verify that your pipeline works as you designed it.
  Take a screenshot of the Circle CI or Jenkins pipeline showing deployment, and a screenshot of your AWS EC2 page showing the newly created (for blue/green) or         modified (for rolling) instances. Make sure you name your instances differently between blue and green deployments.
  Submitting your Project
  Make sure you have taken all the screenshots you need, as directed above, and create a text file with a link to your GitHub repo.

#PROJECT URL






