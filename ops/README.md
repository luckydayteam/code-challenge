# Lucky Day Developer Operations Challenge

## Description 

Provide a HA infrastructure for a single tier web application role that can heal from termination of an instance. The web app server should be able to respond with a unique identifier like its local public ip address. Page response should return both the unique identifier as well as the text 'Health Checker: OK'.

## Goals

This challenge is designed to test your skills with:
* Building into AWS: VPC, ALB, EC2, ASG
* Infrastructure-as-code (Iac) using Cloudformation, Terraform, or Serverless Framework  
* Git

## Requirements

1. Setup a public GitHub repository 'code-challenge' to host the code.
2. Use Clouformation, Terraform, or Serverless Framework to setup infrastructure
3. Setup a [Free-Tier AWS account](https://aws.amazon.com/free/) with your own email and credentials, or use your existing AWS account. 
4. Setup the infrastructure in 'us-west' region with 't3.nano' EC2 instance.

### Bonus Points

1. Return a static image hosted in S3 in the response. Add a CDN with caching in front of the image, but not the web page response.
2. Create a second application that returns the text "Another Health Checker: OK" instead of "Health Checker: OK". Create a script to change the deploymed web application between these two applications without downtime.

## Submission Guidelines

1. Setup a public GitHub repository 'code-challenge' to host the code.
2. Create a README file within the repository that contains the following:
   - Brief walkthrough of your work and approach in steps

3. Email links to your **public GitHub** repo with your name in subject line to [dev-challenge@luckydayapp.com](mailto:dev-challenge@luckydayapp.com)