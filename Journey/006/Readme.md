# STR04-AWS100 - Create an S3 Bucket and store an object in it

<p align="center">
<img src="https://user-images.githubusercontent.com/80279467/175890109-566cd89f-b756-4af3-a001-836b18888432.png"  ></p>

## Cloud Service Provider
- Amazon Web Services

## Difficulty
- Level 100 (Introductory)

## Project's Author(s)
- [Syed Auther](https://twitter.com/syedauther)

## Objectives

### You need to complete the following:

- Using the console, create an S3 bucket
- Upload an object (any file) into the bucket


### You need to answer the following:
- What is Simple Storage Service (S3)?
Amazon S3 or Amazon Simple Storage Service is a service offered by Amazon Web Services that provides object storage through a web service interface. Amazon S3 uses the same scalable storage infrastructure that Amazon.com uses to run its e-commerce network.
## -what is bucket?
A bucket is a container for objects stored in Amazon S3. You can store any number of objects in a bucket and can have up to 100 buckets in your account. To request an increase, visit the Service Quotas Console . Every object is contained in a bucket. For example, if the object named photos/puppy.
## - What is object storage?
Object storage is a computer data storage that manages data as objects, as opposed to other storage architectures like file systems which manages data as a file hierarchy, and block storage which manages data as blocks within sectors and tracks.
## - How is object storage different than block storage?
Object storage is best used for large amounts of unstructured data, especially when durability, unlimited storage, scalability, and complex metadata management are relevant factors for overall performance. Block storage provides low latency and high-performance values in various use cases
## - What is the maximum amount of data that you can store in an S3 bucket? 
The total volume of data and number of objects you can store are unlimited. Individual Amazon S3 objects can range in size from a minimum of 0 bytes to a maximum of 5 TB. The largest object that can be uploaded in a single PUT is 5 GB.
## - What is the maximum file size you can store in an S3 bucket?
The total volume of data and number of objects you can store are unlimited. Individual Amazon S3 objects can range in size from a minimum of 0 bytes to a maximum of 5 TB. The largest object that can be uploaded in a single PUT is 5 GB.
## - By default, are objects in an S3 bucket public?
By default, new buckets, access points, and objects don't allow public access. However, users can modify bucket policies, access point policies, or object permissions to allow public access. S3 Block Public Access settings override these policies and permissions so that you can limit public access to these resources.
## - What are the security best practices regarding S3 buckets?
Top 10 security best practices for securing data in Amazon S3
Block public S3 buckets at the organization level. ...
Use bucket policies to verify all access granted is restricted and specific. ...
Ensure that any identity-based policies don't use wildcard actions. ...
Enable S3 protection in GuardDuty to detect suspicious activities.
## - What is an S3 bucket policy?
An S3 bucket policy is an object that allows you to manage access to specific Amazon S3 storage resources. You can specify permissions for each resource to allow or deny actions requested by a principal (a user or role).
## - What are storage classes in S3?
S3 has six storage classes puprose-built for varying access needs to help you optimize costs. With the S3 Storage Classes, S3 Storage Class Analysis, and S3 Lifecycle policies, you can enable storage cost efficiencies without impacting availability or performance.
## - How is a bucket policy different from an IAM policy? 
 You attach IAM policies to IAM users, groups, or roles, which are then subject to the permissions you've defined. In other words, IAM policies define what a principal can do in your AWS environment. S3 bucket policies, on the other hand, are attached only to S3 buckets

## References
- [Getting Started with S3](https://docs.aws.amazon.com/AmazonS3/latest/gsg/GetStartedWithS3.html)
- [Intro to S3](https://www.youtube.com/watch?v=M_t32mJCXqI)
- [Creating a bucket](https://docs.aws.amazon.com/AmazonS3/latest/gsg/CreatingABucket.html)
- [Uploading your first object into a bucket](https://docs.aws.amazon.com/AmazonS3/latest/gsg/PuttingAnObjectInABucket.html)
- [Bucket Policies](https://docs.aws.amazon.com/AmazonS3/latest/dev/access-policy-language-overview.html)
- [Storage classes in S3](https://aws.amazon.com/s3/storage-classes/)
- [Security breach due to public bucket policies](https://www.bleepingcomputer.com/news/security/540-million-facebook-records-leaked-by-public-amazon-s3-buckets/)

## Costs
- This project is included in the free tier.
- The free tier includes 5GB of Amazon S3 storage in the S3 Standard storage class; 20,000 GET Requests; 2,000 PUT, COPY, POST, or LIST Requests; and 15GB of Data Transfer Out each month.
- An empty bucket does not incur any costs.
- [S3 Pricing after free tier exhaustion](https://aws.amazon.com/s3/pricing/?nc=sn&loc=4)

## Estimated time to complete
- 15 minutes

## Tips
- Each bucket's name has to be unique _globally_, across every single bucket in the world.
- Try to get the URL for the object you uploaded in this task and access it using a browser, you should get an access denied error
- Do not store sensitive information in a bucket that has public access.
- Do not turn on _versioning_ on this bucket, it will be difficult to delete.
