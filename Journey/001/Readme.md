# DEV03-AWS100 —  Install & Configure AWS CLI then create an S3 Bucket
<a href="url"><img src="https://user-images.githubusercontent.com/69337392/175266255-e6768029-3fe4-46f3-9c18-528cb4febeb7.png" height="500" width="262" ></a>

## Introduction

✍️ (Why) Amazon S3 is a program that's built to store, protect, and retrieve data from “buckets” at any time from anywhere on any device. Organizations of any size in any industry can use this service.

## Prerequisite

✍️ (What)
## S3
* Organizing, storing and retrieving data in Amazon S3 focuses on two key components: buckets and objects that work together to create the storage system. As AWS      describes it, an S3 environment is a flat structure — a user creates a bucket; the bucket stores objects in the cloud. 
## CLI (Command Line Interface) 
* The AWS Command Line Interface (AWS CLI) is a unified tool to manage your AWS services. With just one tool to download and configure, you can control multiple AWS services from the command line and automate them through scripts.

## Cloud Service Provider
* Amazon Web Services (AWS)

## Difficulty
Level 100 (Introductory)

## Estimated Time
* 30 - 40 minutes
  
## Project's Author(s)
* [Ariela](https://twitter.com/ari_hacks)

## Objectives

###  You need to complete the following:

* Create an IAM user with a programmatic access type (and Administrator Access) if you do not have one already
* Install AWS CLI 
* Configure AWS credentials locally: `aws configure` 
* Create an S3 bucket: `aws s3 mb s3://<unique-bucket-name>`
* Check the bucket was created: `aws s3 ls`
* Delete the bucket when you are done: `aws s3 rb s3://<unique-bucket-name>`

###  You need to answer the following: 

* How are permissions granted to IAM users?
* What credentials are created when configuring AWS locally and where are they stored? 
* What is the difference between `s3` and `s3api` Commands?
  

## References
* [Using S3 Endpoints](https://aws.amazon.com/blogs/infrastructure-and-automation/best-practices-for-using-amazon-s3-endpoints-in-aws-cloudformation-templates/)
* [Create an IAM user](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_users_create.html)
* [Install AWS CLI on MacOS](https://docs.aws.amazon.com/cli/latest/userguide/install-macos.html) or with Homebrew:  `brew install awscli` `aws --version`
* [Install AWS CLI on Windows](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2-windows.html)
* [Install AWS CLI on Linux](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2-linux.html)
* [Configure AWS locally](https://docs.aws.amazon.com/cli/latest/userguide/cli-configure-quickstart.html)
* [Leveraging the s3 and s3api Commands](https://aws.amazon.com/blogs/developer/leveraging-the-s3-and-s3api-commands/)


## Tips
  - IAM users with programmatic access are given an *access key id* and *secret access key*. After creating a user a *Download.csv* file is generated that contains these values. Download and save the file to access them for setting up AWS locally.
