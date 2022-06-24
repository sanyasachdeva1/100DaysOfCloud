# COM03-AWS100 - Launch a Hello World website on the internet
<p align="center">
<img src="https://user-images.githubusercontent.com/69337392/175494432-e66aa076-38ea-4e68-98ea-faa1edec407c.jpg" height="262" width="700" ></p>


## Introduction

✍️ Why? 
The AWS Amplify Console provides a complete workflow for developing, deploying, and hosting single page web apps or static sites with serverless backends. You can add dynamic functionality to your app with the Amplify Framework, and then deploy it to your end users instantly with the Amplify Console.

## Prerequisite

✍️ What?
* EC2  enables on-demand, scalable computing capacity in the AWS cloud. Amazon EC2 instances eliminate the up-front investment for hardware, and there is no need to maintain any rented hardware. It enables you to build and run applications faster. You can use EC2 in AWS to launch as many virtual servers as you need.

* AWS security group  acts as a virtual firewall for your EC2 instances to control incoming and outgoing traffic. Both inbound and outbound rules control the flow of traffic to and traffic from your instance, respectively.

## Cloud Research

✍️ Possible errors could be- 
  1. Connecting to your instance: Connection timed out
  2. Unable to load key.
  3. User key not recognized by server
  4. Permission denied or connection closed by [instance] port 22
  5. Unprotected private key file
  6. Private key must begin with "-----BEGIN RSA PRIVATE KEY-----" and end with "-----END RSA PRIVATE KEY-----"
  7. Server refused our key or No supported authentication methods available
  8. Cannot ping instance
  9. Server unexpectedly closed network connection
  10. Host key validation failed for EC2 Instance Connect
  11. Can't connect to Ubuntu instance using EC2 Instance Connect
  12. Lost the private key. 

<p align="left">
<img src="https://user-images.githubusercontent.com/69337392/175496440-39bbc42a-bd5a-4149-8d4f-131655186a37.png"></p>

## Try yourself

✍️ Hosting a website using AWS :- 
Step 1: Gathering the Basics.
Step 2: Create a S3 Bucket of your website.
Step 3: Uploading file into your S3 Bucket.
Step 4: Configure the settings of your S3 Bucket.
Step 5: Hosting your Website.

### Important steps:- 
1. Launch a linux based EC2 instance in any one region of your choice in a public subnet
2. Setup a security group that allows http/https connections from the Internet, and ssh from your IP address
3. SSH into the EC2 instance
4. Setup a webserver on the EC2 instance
5. Add a simple hello world header to the index.html file
6. Hit the public IP address from a browser and confirm the site is served

## References
- [What Is Amazon EC2?](https://aws.amazon.com/ec2/faqs/)
- [Security Groups](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/ec2-security-groups.html#:~:text=A%20security%20group%20acts%20as,one%20or%20more%20security%20groups.)
- [Installing httpd](http://httpd.apache.org/docs/2.4/install.html)
- [ssh into ec2 - linux](https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/AccessingInstancesLinux.html)

## Ideas
- For windows users [Download and install Putty](https://www.chiark.greenend.org.uk/~sgtatham/putty/latest.html)
- Connecting to a Linux EC2 instance from Windows is not possible natively, you will need an ssh client such as Putty to connect , and you will need to follow these steps to [ssh into ec2 from windows](https://stackoverflow.com/questions/5264945/ssh-to-ec2-linux-instance-from-windows)
- You can also launch non linux EC2 instances for example windows servers, for which you will need to RDP into.  

## Tips
- Use t2.micro instances from the free tier as it will suffice for this static site 
- Use the default setting on the storage screen as 8GB of EBS storage will be enough for this project.
