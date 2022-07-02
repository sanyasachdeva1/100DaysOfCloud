# COM04-AWS100 - Push a Docker image to Amazon ECR repository

## Cloud Service Provider

- Amazon Web Services

## Difficulty

- Level 100 (Introductory)

## Project's Author(s)

- [Johan Rin](https://twitter.com/johanrin)

## Architecture 
<p align="center">
<img src="https://user-images.githubusercontent.com/80279467/176993578-1b5fa56b-2b7c-4999-9d23-93ff747cbfe3.png"  ></p>

### Prerequisites

- A Docker image

### You need to complete the following:

- Create your Amazon ECR repository
- Authenticate your Docker to Amazon ECR
- Tag your Docker image with the Amazon ECR repository
- Push your image to Amazon ECR

### You need to answer the following:

## - What is the URL for your default registry?
The URL for your default private registry is https:// aws_account_id . dkr. ecr. region 

## - What is a _Tag immutability_ in Amazon ECR repository?
Amazon ECR Tag Immutability enables customers to rely on the descriptive tags of an image as a reliable mechanism to track and uniquely identify images. Prior to this enhancement, tags could be overwritten requiring developers to use the Image SHA to know which image was being deployed.

## - What is a _Scan on push_ in Amazon ECR repository?
Amazon ECR Scan on Push helps you identify software vulnerabilities within your container images by checking each image against an aggregated set of Common Vulnerabilities and Exposures (CVEs)

## - How long an _Authorization Token_ is valid?
The access token is set with a reasonably lower expiration time of 30 mins. The refresh token is set with a very long expiration time of 200 days. If the traffic to this API is 10 requests/second, then it can generate as many as 864,000 tokens in a day.

## - How many tags per image can you apply in Amazon ECR?
Maximum number of tags per repository – 50.

## References

- [Get started with Docker](https://docs.docker.com/get-started/)
- [How to build a Docker image](https://www.youtube.com/watch?v=6Er8MAvTWlI)
- [Creating a Repository](https://docs.aws.amazon.com/AmazonECR/latest/userguide/repository-create.html)
- [Registry Authentication](https://docs.aws.amazon.com/AmazonECR/latest/userguide/Registries.html#registry_auth)
- [Pushing an image](https://docs.aws.amazon.com/AmazonECR/latest/userguide/docker-push-ecr-image.html)

## Costs

- Included in the Free Tier

## Estimated time to complete

- 30 minutes - only if you already have a Docker image
