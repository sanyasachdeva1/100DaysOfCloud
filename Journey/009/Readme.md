# COM04-AWS200 - Deploy a Docker container image on AWS Fargate

## Cloud Service Provider

- Amazon Web Services

## Difficulty

- Level 200 (Intermediate)

## Project's Author(s)

- [Johan Rin](https://twitter.com/johanrin)

## Architecture
<p align="center"> <img src="https://user-images.githubusercontent.com/80279467/176993768-5ef28cde-22e3-42aa-9025-1e9ba45ffd40.png"  ></p>

### Prerequisites

- [Push a Docker image to Amazon ECR repository](./COM04-AWS100.md)

### You need to complete the following:

- Configure your container with your Docker image
- Configure your task definition
- Define your service
- Configure your cluster

### You need to answer the following:

## - What is a _container_?
A container is any receptacle or enclosure for holding a product used in storage, packaging, and transportation, including shipping. Things kept inside of a container are protected on several sides by being inside of its structure.

## - What is the difference between Soft memory limit and Hard memory limit for a custom container?
IIRC the soft limit is how much memory the scheduler reserves on an instance for the task to run, and the hard limit is how much memory a container can use before it is murdered.26

## - What is the name of the default task execution role?
The task execution role grants the Amazon ECS container and Fargate agents permission to make AWS API calls on your behalf. The task execution IAM role is required depending on the requirements of your task. You can have multiple task execution roles for different purposes and services associated with your account.

## - What does a task size allow?
In Amazon ECS, there are two resource metrics used for capacity: CPU and memory. CPU is measured in units of 1/1024 of a full vCPU (where 1024 units is equal to 1 whole vCPU). Memory is measured in megabytes. In your task definition, you can declare resource reservations and limits.

## - What is a _service_?
A service is an " act or use for which a consumer, firm, or government is willing to pay." Examples include work done by barbers, doctors, lawyers, mechanics, banks, insurance companies, and so on. Public services are those that society as a whole pays for.

## - Which load balancer type Fargate can handle?
Amazon ECS services hosted on AWS Fargate support the Application Load Balancer and Network Load Balancer load balancer types. Application Load Balancers are used to route HTTP/HTTPS (or layer 7) traffic. Network Load Balancers are used to route TCP or UDP (or layer 4) traffic

## - How many security groups are created by default if you use a load balancer?
Elastic Load Balancing creates only one such security group per AWS account, with a name of the form default_elb_ id (for example, default_elb_fc5fbed3-0405-3b7d-a328-ea290EXAMPLE ). Subsequent load balancers that you create in the default VPC also use this security group

## - What is a _cluster_?
A computer cluster is a set of computers that work together so that they can be viewed as a single system. Unlike grid computers, computer clusters have each node set to perform the same task, controlled and scheduled by software.

## - What are cluster names limitations?
I went through the Active Directory naming conventions. It says, for proper name resolution, the recommended limit is 15 characters

## References

- [Getting started with Amazon ECS using Fargate](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/getting-started-fargate.html)
- [Deploy Docker Containers](https://aws.amazon.com/getting-started/hands-on/deploy-docker-containers/)
- [How Amazon ECS manages CPU and memory resources](https://aws.amazon.com/blogs/containers/how-amazon-ecs-manages-cpu-and-memory-resources/)
- [Amazon ECS Task Execution IAM Role](https://docs.aws.amazon.com/AmazonECS/latest/developerguide/task_execution_IAM_role.html)

## Costs

- Included in the Free Tier

## Estimated time to complete

- 45 minutes - only if you already have a Docker image
