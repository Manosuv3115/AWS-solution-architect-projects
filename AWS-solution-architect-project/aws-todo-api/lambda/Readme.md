
## Table of Contents
- [Overview](#overview)
- [Architecture](#architecture)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [Deployment](#deployment)
- [Screenshots](#screenshots)
- [License](#license)

## Overview

Build a rest API to manage tasks (read,Create,delete).

## Architecture

AWS services used:

AWS Lambda (function logic)

API Gateway (exposes HTTP endpoints)

DynamoDB (stores data)

## Technologies Used

- Python
- AWS Services (API Gateway, Lambda, Dynamo DB)

## Getting Started

# Create Lambda Function in AWS Console
Go to AWS Lambda

Click Create function

Choose Author from scratch

Runtime: Python 3.9

Function name: taskHandler

Create

In the Code editor, paste task_handler.py content

# Create DynamoDB Table

Go to AWS DynamoDB

Create a table:

Table name: Tasks

Primary key: taskId (String)

# Create API Gateway

Go to API Gateway

Create a new HTTP API

Add integration → Lambda function → select taskHandler

Create route: GET /tasks

Deploy the API

Copy the Invoke URL

