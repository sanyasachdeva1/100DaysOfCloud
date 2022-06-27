# SEC04-AWS100 — Create an IAM user

<p align="center" >
<img src="https://user-images.githubusercontent.com/69337392/175890661-f87210ba-c6ce-43ec-ab7f-5896e410a7b0.png" height="500" width="600" ></p>

## Introduction

✍️ Why?
- An AWS Identity and Access Management (IAM) user is an entity that you create in AWS to represent the person or application that uses it to interact with AWS. A user in AWS consists of a name and credentials. An IAM user with administrator permissions is not the same thing as the AWS account root user.

## Prerequisite

✍️ What?
- IAM user limit is 5000 per AWS account.
- In the AWS Management Console section, under Delegate console access, choose the IAM role name for the existing IAM role that you want to assign users to. If the role has not yet been created, see Creating a new role. On the Selected role page, under Manage users and groups for this role, choose Add.

### What is IAM user and root user in AWS?
 1. There are two different types of users in AWS. You are either the account owner (root user) or you are an AWS Identity and Access Management (IAM) user. The root user is created when the AWS account is created. 
 2. IAM users are created by the root user or an IAM administrator for the account.

## Use Case
![aws-iam-sso-5](https://user-images.githubusercontent.com/69337392/175891142-c313ceee-d18b-4247-beaa-55bf46a88cf1.png)

## Cloud Service Provider

* Amazon Web Services

## Difficulty
* Level 100 (Introductory)

## Estimated time:
 * 1 hour

## Cost
* IAM is a free service

## Project's Author(s)
* [Syed Auther](https://twitter.com/syedauther)

## Objectives

### You need to complete the following:

* Create a new user in IAM with console access
* Add the user to an Admin group 
  * Create a new group called "Admins"
  * Add the `AdministratorAccess` managed policy to the new group
  * Add your new user to the "Admins" group
* Enable MFA for the root user
* Apply an IAM password policy that follows security best practices



### You need to answer the following: 

* What is Identity and Access Management (IAM)? 
* What is a root user?
* How is a root user different from an Admin user? 
* What is console access and programmatic access? 
* What is the access key and secret key? 
* What is MFA and why is it important?
* What are policies and how can you create them?
* What are roles and how can you create them?
* What is the difference between a role and a policy?
* What is a user group? 
* What are some good security practices for password policies? 

## References

* [Creating Your First IAM Admin User and Group](https://docs.aws.amazon.com/IAM/latest/UserGuide/getting-started_create-admin-group.html)
* [Security Best Practices in IAM](https://docs.aws.amazon.com/IAM/latest/UserGuide/best-practices.html)
* [Root user in AWS](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_root-user.html)
* [Setting an IAM password policy](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_credentials_passwords_account-policy.html?icmpid=docs_iam_console)
* [IAM Policy examples](https://docs.aws.amazon.com/IAM/latest/UserGuide/access_policies_examples.html)
* [About IAM Roles](https://docs.aws.amazon.com/IAM/latest/UserGuide/id_roles.html)


## Tips
* Managed policies are created and maintained by AWS. A managed policy has a small, orange box on the left side of the policy's name.
* Use the [Google Authenticator](https://play.google.com/store/apps/details?id=com.google.android.apps.authenticator2) app for MFA.
* Do not ever commit, add or push any of your access and secret keys to source control systems like git. You must also never share or make your access keys public in any way shape or form. If you accidentaly have done so, make sure to delete the access and secret keys immediately in your console and generate new ones.
* By default, IAM users are not allowed access to the Billing console. It has to be enabled seperately by using the root user under "My Account".
