# Documentation of hackathon project1 
Please fix it to get your unsecured highly available apache website to work.This DevOps Hackathon template will create ELB Security Group, ELB, ELB Listener,Target Group, Launch Configuration and Autoscaling group.

### Requirement of hackathon project 1
1. # HACKATHON STUDENT NOTE:

Your colleague has provided you with a CloudFormation template to deploy an insecure, highly available Apache website.

Your task is to troubleshoot and fix the CloudFormation template.

To test the application, deploy the template on the CloudFormation console and access the load balancer's DNS name using a web browser of your choice. 
# Hint: You do not need to SSH into the EC2 web servers.


# Note:

1) The CloudFormation template should be executed on the CloudFormation console.
2) The application should be highly available and accessible on port 80.
3) There is no database associated with the application.
4) The instance type to be used is t3.micro.

2. # Update the broken template
 We first created a new template call "hackaton-fixed-template" 
1) add a t3.micro
2) Change the ami of us-east-1 to the one we have in our console 
3) Change the port number from 443(https) to port 80(http) as recommended in the requirement
4) Updated the cird bloque to 0.0.0.0/0 
5) Commented the dbsecurity group( not needed in this)
6) Change the security group from dbsecurity to elbsecurity 
7) Change the minimum size to atleast 2 for highly avaiable 

