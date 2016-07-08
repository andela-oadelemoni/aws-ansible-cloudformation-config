# AWS Ansible Cloudformation Config
Ansible script for AWS Cloudformation, S3 website, and Autoscaling group configuration

### Summary
This Ansible Playbook does the following:
1. Creates an S3 bucket, upload static website to it, and set needed permissions
2. Creates an AMI based on a given Instance ID.
3. Creates a VPC with a private and public subnet based on a cloudformation template
4. Launches an Instance, based on the created AMI above, into the private subnet created
5. Creates an Autoscaling Group based on the created AMI.



### Steps
1. Open vars.yml and enter the required variables for the script to run
2. Create a credentials.yml file locally with the following content:
```
aws_access_key: <enter access key>
aws_secret_key: <enter secret key>
```
3. Run aws_config.yml.


