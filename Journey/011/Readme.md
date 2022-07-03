# COM04-AWS400 - Create a cluster of virtual machines using docker swarm

<p align="center" >
<img src="https://user-images.githubusercontent.com/69337392/177027792-1868ce70-6920-47fa-82c7-6fd7c49ce44e.jpeg" height="400" width="800" ></p>

## Introduction

✍️ A docker swarm is comprised of a group of physical or virtual machines operating in a cluster. When a machine joins the cluster, it becomes a node in that swarm.

## Prerequisite

✍️ Docker Swarm is the Docker-native solution for deploying a cluster of Docker hosts. You can use it to quickly deploy a cluster of Docker hosts running either on your local machine or on supported cloud platforms.

## Cloud Service Provider

- Amazon Web Services

## Difficulty

- Level 400 (Expert)

## Project's Author(s)

[Karan Gauswami](https://github.com/KaranGauswami)

## Objectives

### You need to complete the following:

- Create an EC2 Instance with user data script to install Docker
- Setup that EC2 Instance as a manager node
- Create multiple instances (2 to 3) with user data script to create worker nodes and join them with manager node
- Start any service like nginx to test our Swarm Cluster
- Scale that service to multiple nodes
- Delete all the resources you created after completion

### You need to answer the following:

- How to check status of Docker nodes ?
- What behaviour is expected if one of the worker or manager nodes went down ?
- How to get state of all the containers running on different nodes ?
- How to get token to add more workers and managers ?

## References

- [Running commands on your Linux instance at launch](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/user-data.html)
- [Install Docker](https://docs.docker.com/engine/install/ubuntu/)
- [Get Started with Docker Swarm](https://docs.docker.com/engine/swarm/swarm-tutorial)

## Costs

- Included in the Free Tier
- \$1-2 per hour running

## Estimated time to complete

- 4-5 hours

## Tips

- Use t2.micro instances for creating nodes to avoid unexpected charges.
- To add more manager or worker nodes, it is not required to SSH into the new instance. Utilize the "user data" functionality.
- Only allow incoming SSH traffic in security groups for the instances that require it.
