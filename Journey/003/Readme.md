# BIL02-AWS100 — Create a Cost Budget
<p align="center" >
<img src="https://user-images.githubusercontent.com/80279467/175764909-8044f5c2-3894-4550-920c-2d015b7ab1bb.png" height="300" width="700" ></p>

## Introduction

✍️ (Why?)
- AWS Budgets allows you to set custom budgets to track your cost and usage from the simplest to the most complex use cases. With AWS Budgets, you can choose to be alerted by email or SNS notification when actual or forecasted cost and usage exceed your budget threshold, or when your actual RI and Savings Plans' utilization or coverage drops below your desired threshold. With AWS Budget Actions, you can also configure specific actions to respond to cost and usage status in your accounts, so that if your cost or usage exceeds or is forecasted to exceed your threshold, actions can be executed automatically or with your approval to reduce unintentional over-spending. 

## Prerequisite

✍️ (What?)
- There are three fundamental drivers of cost with AWS: compute, storage, and outbound data transfer. These characteristics vary somewhat, depending on the AWS product and pricing model you choose.In most cases,there is no charge for inbound data transfer or for data transfer between other AWS services within the same AWS Region. There are some exceptions,so be sure to verify data transfer rates before you begin to use the AWS service.Outbound data transfer is aggregated across servicesand then charged at the outbound data transfer rate. This charge appears on the monthly statement as AWS Data Transfer Out. AWS Academy Cloud FoundationsModule 2: Cloud Economics and Billing© 2022 Amazon Web Services, Inc. or its affiliates. All rights reserved.

## Cloud Service Provider
Amazon Web Services (AWS)

## Difficulty
Level 100 (Introductory)

## Estimated Time
20 - 40 minutes 
  
## Project's Author(s)
[Ariela](https://twitter.com/ari_hacks)

## Objectives
###  You need to complete the following:

Create a cost budget 

###  You need to answer the following: 

In order for IAM users to create budgets in the Billing and Cost Management console what else must these users be allowed to do? 

- This table summarizes the permissions that allow or deny IAM users access to your billing information and tools. For examples of policies that use these permissions, see AWS Billing policy examples.

### In addition to the console how else can you create budgets? 
## Step 1: Calculate your net income
The foundation of an effective budget is your net income. That’s your take-home pay—total wages or salary minus deductions for taxes and employer-provided programs such as retirement plans and health insurance. Focusing on your total salary instead of net income could lead to overspending because you’ll think you have more available money than you do. If you’re a freelancer, gig worker, contractor or are self-employed, make sure to keep detailed notes of your contracts and pay in order to help manage irregular income.

## Step 2: Track your spending
Once you know how much money you have coming in, the next step is to figure out where it’s going. Tracking and categorizing your expenses can help you determine what you are spending the most money on and where it might be easiest to save.

## Step 3: Set realistic goals
Before you start sifting through the information you’ve tracked, make a list of your short- and long-term financial goals. Short-term goals should take around one to three years to achieve and might include things like setting up an emergency fund or paying down credit card debt.

## Step 4: Make a plan
This is where everything comes together: What you’re actually spending vs. what you want to spend. Use the variable and fixed expenses you compiled to get a sense of what you’ll spend in the coming months. Then compare that to your net income and priorities. Consider setting specific—and realistic—spending limits for each category of expenses.

## Step 5: Adjust your spending to stay on budget
Now that you’ve documented your income and spending, you can make any necessary adjustments so that you don’t overspend and have money to put toward your goals.

## step 6: Review your budget regularly
Once your budget is set, it’s important to review it and your spending on a regular basis to be sure you are staying on track. Few elements of your budget are set in stone: You may get a raise, your expenses may change or you may reach a goal and want to plan for a new one. Whatever the reason, get into the habit of regularly checking in with your budget following the steps above.

## What are the different types of costs that make up a cost budget? 
Fixed expenses, savings expenses, and variable costs are the three categories that make up your budget, and are vitally important when learning to manage your money properly. When you’ve committed to living on a budget, you must know how to put your plan into action.

## What are the different options for setting budget alerts? 
Sign in to the AWS Management Console and open the AWS Cost Management console at https://console.aws.amazon.com/cost-management/home . In the navigation pane, choose Budgets. At the top of the page, choose Create budget. For Choose budget type, choose Savings Plans budget.  

## References

[Create a cost budget](https://docs.aws.amazon.com/awsaccountbilling/latest/aboutv2/budgets-create.html#create-cost-budget)
