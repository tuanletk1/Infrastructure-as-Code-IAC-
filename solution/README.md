# Udacity Cloud DevOps Engineer

## Deploy a high-availability web app using CloudFormation 

### Problem Statement 
* Your company is creating an Facebook clone called Udagram. Developers want to deploy thier application to the AWS infrastructure. They pushed thier latest contribution to a public S3 Bucket.  

* You have been tasked with provisioning the required infrastructure and deploying thier latest contribution files which are located in a public S3 Bucket to the Apache Web Server running on an EC2 instance, along with the necessary supporting software.

* This needs to be automated so that the infrastructure can be discarded as soon as the testing team finishes their tests and gathers their results.


### Diagram of the Infrastructure
![Infrastructure-Diagram](/Deployment%20screenshots/Deploy%20a%20high-availability%20web%20app%20using%20CloudFormation.png)

### Deployment Instruction for the Infrastructure

#### Run the network setup command
```
$ sh create.sh network network.yml network-parameters.json 
```
#### Run the server setup command
```
$ sh create.sh server servers.yml server-parameters.json
```

### Output of Project
![Website-of-the-project](/Deployment%20screenshots/19.%20website%20LB-EC2-s3%20connectivity%20check.png)

### Access the link in the server output
[http://server-webap-5lm8xj3ygdf3-604021572.us-east-1.elb.amazonaws.com/](http://server-webap-5lm8xj3ygdf3-604021572.us-east-1.elb.amazonaws.com/)