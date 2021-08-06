# Udacity Nanodegree Project 2

## Overview

Deploys an HA Application Tier with CloudFormation. Refer to the included diagram image for the resources it deploys. The project advertises an Instagram clone (called Udagram) that is available on a public S3 with JavaScript and HTML files, but I have no idea where these files are created nor where to grab them from


## Folder Structure
```
├── stack.yaml									# CloudFormation template file
├── udacity-project-2.drawio		# raw XML file used to generate the architecture diagram
└── udacity-project-2.png				# the architecture diagram
```

## Running
* Using the AWS CLI (I prefer to use the interactive CLI [aws-shell](https://github.com/awslabs/aws-shell)):
```
aws cloudformation create-stack --stack-name udacity-proj2 --template-body file://stack.yaml --capabilities CAPABILITY_IAM
```
* Using the AWS Web Console: go to Cloudformation and upload the `stack.yaml` file
