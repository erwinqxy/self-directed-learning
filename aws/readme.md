# AWS Cheatsheet

## AWS S3

![S3 Diagram](./image/s3-diagram.png)

- S3 is AWS' solution for object storage, where S3 buckets are like a hard drive in the cloud for static files.
- You can have unlimited number of objects in a bucket and any fiile type.
- If you upload an object with a key name that already exists in a versioning-enabled bucket, Amazon S3 creates another version of the object instead of replacing the existing object.
- Since browsers ultimately download files to use them, we can use S3 as a way to host static websites
- Operations available:
  - Upload an object in a single operation by using the AWS SDKs, REST API, or AWS CLI – With a single PUT operation, you can upload a single object up to 5 GB in size.
  - Upload a single object by using the Amazon S3 console – With the Amazon S3 console, you can upload a single object up to 160 GB in size.

### Use Cases

- Build a data lake
- Back up and restore critical data
- Archive data at the lowest cost
- Run cloud-native applications

### Example - Deploy a static website with AWS S3 and CloudFront

- S3 offers a configuration option that allows us to serve a website from a simple bucket
- CloudFront is a CDN (content delivery network) service that works alongside S3 to improve website performance. While S3 hosts the website in a bucket, CloudFront acts as a cached distributed network layer positioned in front of the bucket. This setup enables faster delivery of website content to visitors' browsers compared to accessing it directly from S3.

### References

- [Amazon S3](https://aws.amazon.com/s3/)
- [Uploading objects](https://docs.aws.amazon.com/AmazonS3/latest/userguide/upload-objects.html)
- [Hosting a static website on Amazon S3](https://docs.aws.amazon.com/AmazonS3/latest/userguide/WebsiteHosting.html)

## AWS Lambda

- Run code without thinking about servers or clusters
- Lambdas functions run in the cloud, so we dont have to worry about any of resources that make that function run
- Run code without provisioning or managing infrastructure. Simply write and upload code as a .zip file or container image.

### Use Cases

- Read and write data to S3 or database
- Process data at scale
- Run interactive web and mobile backends
- Enable powerful ML insights
- Create event-driven applications

### References

- [AWS Lambda](https://aws.amazon.com/lambda/)
- [AWS Lambda course](https://egghead.io/lessons/aws-wtf-is-aws-lambda)

## AWS EC2 (Elastic Compute Cloud)

- Spin up a server with a variety of available conifurations

### Use Cases

- Run cloud-native and enterprise applications
- Train and deploy ML applications

### References

- [AWS Lambda](https://aws.amazon.com/ec2/)
- [Spin up a remote server on AWS](https://www.freecodecamp.org/news/getting-started-with-server-administration-on-aws/)
- [Serverless](https://www.serverless.com/)
