**AWS Certified Solutions Architect Associate Practice Test**

# A development team needs to run up a few lab servers on a weekend for a new project. The servers will need to run uninterrupted for a few hours. Which EC2 pricing option would be most suitable?   

## CORRECT: "On-Demand" is the correct answer.

 
# An Amazon Elastic File System (EFS) has been created to store data that will be accessed by a large number of Amazon EC2 instances. The data is sensitive and a Solutions Architect is creating a design for security measures to protect the data. It is required that network traffic is restricted correctly based on firewall rules and access from hosts is restricted by user or group. How can this be achieved with Amazon EFS? (choose 2)

## CORRECT: "Use POSIX permissions to control access from hosts by user or group" is the correct answer.

## CORRECT: "Use EFS Security Groups to control network traffic" is the correct answer.


# A company needs to ensure that they can failover between AWS Regions in the event of a disaster seamlessly with minimal downtime and data loss. The applications will run in an active-active configuration. Which DR strategy should a Solutions Architect recommend?

## CORRECT: "Multi-site" is the correct answer.


# An Amazon EC2 instance has been launched into an Amazon VPC. A Solutions Architect needs to ensure that instances have both a private and public DNS hostnames. Assuming settings were not changed during creation of the VPC, how will DNS hostnames be assigned by default? (choose 2)


## CORRECT: "In a default VPC instances will be assigned a public and private DNS hostname" is the correct answer.
## CORRECT: "In a non-default VPC instances will be assigned a private but not a public DNS hostname" is the correct answer.


# Several Amazon EC2 Spot instances are being used to process messages from an Amazon SQS queue and store results in an Amazon DynamoDB table. Shortly after picking up a message from the queue AWS terminated the Spot instance. The Spot instance had not finished processing the message. What will happen to the message?

## CORRECT: "The message will become available for processing again after the visibility timeout expires" is the correct answer.


# An application uses an Amazon RDS database and Amazon EC2 instances in a web tier. The web tier instances must not be directly accessible from the internet to improve security. How can a Solutions Architect meet these requirements?

## CORRECT: "Launch the EC2 instances in a private subnet and create an Application Load Balancer in a public subnet" is the correct answer.

 
# A company is investigating ways to analyze and process large amounts of data in the cloud faster, without needing to load or transform the data in a data warehouse. The data resides in Amazon S3. Which AWS services would allow the company to query the data in place? (choose 2)

## CORRECT: "Amazon S3 Select" is a correct answer.
## CORRECT: "Amazon RedShift Spectrum" is also a correct answer.

 
# Three AWS accounts are owned by the same company but in different regions. Account Z has two AWS Direct Connect connections to two separate company offices. Accounts A and B require the ability to route across account Z’s Direct Connect connections to each company office. A Solutions Architect has created an AWS Direct Connect gateway in account Z. How can the required connectivity be configured?

## CORRECT: "Associate the Direct Connect gateway to a virtual private gateway in account A and B" is the correct answer.


# A legacy application is being migrated into AWS. The application has a large amount of data that is rarely accessed. When files are accessed they are retrieved sequentially. The application will be migrated onto an Amazon EC2 instance. What is the LEAST expensive EBS volume type for this use case?

## CORRECT: "Cold HDD (sc1)" is the correct answer.


# A company is transitioning their web presence into the AWS cloud. As part of the migration the company will be running a web application both on-premises and in AWS for a period of time. During the period of co-existence the client would like 80% of the traffic to hit the AWS-based web servers and 20% to be directed to the on-premises web servers. What method can a Solutions Architect use to distribute traffic as requested?

## CORRECT: "Use Route 53 with a weighted routing policy and configure the respective weights" is the correct answer.


# A Solutions Architect is designing the disk configuration for an Amazon EC2 instance. The instance needs to support a MapReduce process that requires high throughput for a large dataset with large I/O sizes. Which Amazon EBS volume is the MOST cost-effective solution for these requirements?

## CORRECT: "EBS Throughput Optimized HDD" is the correct answer.

# A Solutions Architect has created an AWS Organization with several AWS accounts. Security policy requires that use of specific API actions are limited across all accounts. The Solutions Architect requires a method of centrally controlling these actions. What is the SIMPLEST method of achieving the requirements?

## CORRECT: "Create a service control policy in the root organizational unit to deny access to the services or actions" is the correct answer.


# An Amazon EC2 instance behind an Elastic Load Balancer (ELB) is in the process of being de-registered. Which ELB feature is used to allow existing connections to close cleanly?

## CORRECT: "Connection Draining" is the correct answer.


# A Solutions Architect needs to upload a large (2GB) file to an S3 bucket. What is the recommended way to upload a single large file to an S3 bucket?

## CORRECT: "Use Multipart Upload" is the correct answer.


# Some data has become corrupted in an Amazon RDS database. A Solutions Architect plans to use point-in-time restore to recover the data to the last known good configuration. Which of the following statements is correct about restoring an RDS database to a specific point-in-time? (choose 2)

## CORRECT: "You can restore up to the last 5 minutes" is a correct answer.
## CORRECT: "The default DB security group is applied to the new DB instance" is also a correct answer.


# A large multi-national client has requested a design for a multi-region database. The master database will be in the EU (Frankfurt) region and databases will be located in 4 other regions to service local read traffic. The database should be a managed service including the replication. The solution should be cost-effective and secure. Which AWS service can deliver these requirements?

## CORRECT: "RDS with cross-region Read Replicas" is the correct answer.


# A company runs a web-based application that uses Amazon EC2 instances for the web front-end and Amazon RDS for the database back-end. The web application writes transaction log files to an Amazon S3 bucket and the quantity of files is becoming quite large. It is acceptable to retain the most recent 60 days of log files and permanently delete the rest. Which action can a Solutions Architect take to enable this to happen automatically?

## CORRECT: "Use an S3 lifecycle policy with object expiration configured to automatically remove objects that are more than 60 days old" is the correct answer.


# A customer is deploying services in a hybrid cloud model. The customer has mandated that data is transferred directly between cloud data centers, bypassing ISPs. Which AWS service can be used to enable hybrid cloud connectivity?


## CORRECT: "AWS Direct Connect" is the correct answer.

# A company has a fleet of Amazon EC2 instances behind an Elastic Load Balancer (ELB) that are a mixture of c4.2xlarge instance types and c5.large instances. The load on the CPUs on the c5.large instances has been very high, often hitting 100% utilization, whereas the c4.2xlarge instances have been performing well. What should a Solutions Architect recommend to resolve the performance issues?

## CORRECT: "Change the configuration to use only c4.2xlarge instance types" is the correct answer.


# An application receives a high traffic load between 7:30am and 9:30am daily. The application uses an Auto Scaling group to maintain three instances most of the time but during the peak period it requires six instances. How can a Solutions Architect configure Auto Scaling to perform a daily scale-out event at 7:30am and a scale-in event at 9:30am to account for the peak load?

## CORRECT: "Use a Scheduled scaling policy" is the correct answer.


# A web application receives order processing information from customers and places the messages on an Amazon SQS queue. A fleet of Amazon EC2 instances are configured to pick up the messages, process them, and store the results in a DynamoDB table. The current configuration has been resulting in a large number of empty responses to ReceiveMessage API requests. A Solutions Architect needs to eliminate empty responses to reduce operational overhead. How can this be done? 


## CORRECT: "Configure Long Polling to eliminate empty responses by allowing Amazon SQS to wait until a message is available in a queue before sending a response" is the correct answer.

# A Solutions Architect has logged into an Amazon EC2 Linux instance using SSH and needs to determine a few pieces of information including what IAM role is assigned, the instance ID and the names of the security groups that are assigned to the instance. From the options below, what would be the best source of this information?

Instance metadata is available at http://169.254.169.254/latest/meta-data.
## CORRECT: "Metadata" is the correct answer.


# An application is generating a large amount of clickstream events data that is being stored on S3. The business needs to understand customer behaviour and want to run complex analytics queries against the data. Which AWS service can be used for this requirement?

## CORRECT: "Amazon RedShift" is the correct answer.


# An application uses a MySQL database running on an Amazon EC2 instance. The application generates high I/O and constant writes to a single table on the database. Which Amazon EBS volume type will provide the MOST consistent performance and low latency?

## CORRECT: "Provisioned IOPS SSD (io1)" is the correct answer.


# A large quantity of data that is rarely accessed is being archived onto Amazon Glacier. Your CIO wants to understand the resilience of the service. Which of the statements below is correct about Amazon Glacier storage?  (choose 2) 

## CORRECT: "Provides 99.999999999% durability of archives" is the correct answer.
## CORRECT: "Data is resilient in the event of one entire Availability Zone destruction" is the correct answer.


# A Solutions Architect has created a new security group in an Amazon VPC. No rules have been created. Which of the statements below are correct regarding the default state of the security group? (choose 2)

## CORRECT: "There is an outbound rule that allows all traffic to all IP addresses" is the correct answer.
## CORRECT: "There are no inbound rules and traffic will be implicitly denied" is the correct answer.


# A company needs to capture detailed information about all HTTP requests that are processed by their Internet facing Application Load Balancer (ALB). The company requires information on the requester, IP address, and request type for analyzing traffic patterns to better understand their customer base. Which actions should a Solutions Architect recommend?

## CORRECT: "Enable Access Logs and store the data on S3" is the correct answer.


# A customer has requested some advice on how to implement security measures in their Amazon VPC. The client has recently been the victim of some hacking attempts. The client wants to implement measures to mitigate further threats. The client has explained that the attacks always come from the same small block of IP addresses. What would be a quick and easy measure to help prevent further attacks?

## CORRECT: "Use a Network ACL rule that denies connections from the block of IP addresses" is the correct answer.


# An on-premise data center will be connected to an Amazon VPC by a hardware VPN that has public and VPN-only subnets. The security team has requested that traffic hitting public subnets on AWS that’s destined to on-premise applications must be directed over the VPN to the corporate firewall. How can this be achieved?

## CORRECT: "In the public subnet route table, add a route for your remote network and specify the virtual private gateway as the target" is the correct answer.


# A fleet of Amazon EC2 instances running Linux will be launched in an Amazon VPC. An application development framework and some custom software must be installed on the instances. The installation will be initiated using some scripts. What feature enables a Solutions Architect to specify the scripts the software can be installed during the EC2 instance launch?

## CORRECT: "User Data" is the correct answer.


# A Solutions Architect needs to capture information about the traffic that reaches an Amazon Elastic Load Balancer. The information should include the source, destination, and protocol. What is the most secure and reliable method for gathering this data?

## CORRECT: "Create a VPC flow log for each network interface associated with the ELB" is the correct answer.


# A company has launched a multi-tier application architecture. The web tier and database tier run on Amazon EC2 instances in private subnets within the same Availability Zone. Which combination of steps should a Solutions Architect take to add high availability to this architecture? (Select TWO.)

## CORRECT: "Create an Amazon EC2 Auto Scaling group and Application Load Balancer (ALB) spanning multiple AZs" is a correct answer.
## CORRECT: "Create new private subnets in the same VPC but in a different AZ. Migrate the database to an Amazon RDS multi-AZ deployment" is also a correct answer.


# An on-premises server runs a MySQL database and will be migrated to the AWS Cloud. The company require a managed solution that supports high availability and automatic failover in the event of the outage of an Availability Zone (AZ). Which solution is the BEST fit for these requirements?

## CORRECT: "Use the AWS Database Migration Service (DMS) to directly migrate the database to an Amazon RDS MySQL Multi-AZ deployment" is the correct answer.


# A tool needs to analyze data stored in an Amazon S3 bucket. Processing the data takes a few seconds and results are then written to another S3 bucket. Less than 256 MB of memory is needed to run the process. What would be the MOST cost-effective compute solutions for this use case?

## CORRECT: "AWS Lambda functions" is the correct answer.


# The load on a MySQL database running on Amazon EC2 is increasing and performance has been impacted. Which of the options below would help to increase storage performance? (choose 2)

## CORRECT: "Use Provisioned IOPS (I01) EBS volumes" is a correct answer.
## CORRECT: "Use EBS optimized instances" is also a correct answer.


# A Solutions Architect is deploying a production application that will use several Amazon EC2 instances and run constantly on an ongoing basis. The application cannot be interrupted or restarted. Which EC2 pricing model would be best for this workload?

## CORRECT: "Reserved instances" is the correct answer.


# A Solutions Architect created a new IAM user account for a temporary employee who recently joined the company. The user does not have permissions to perform any actions, which statement is true about newly created users in IAM?

## CORRECT: "They are created with no permissions" is the correct answer.

 
# A financial services company regularly runs an analysis of the day’s transaction costs, execution reporting, and market performance. The company currently uses third-party commercial software for provisioning, managing, monitoring, and scaling the computing jobs which utilize a large fleet of EC2 instances. The company is seeking to reduce costs and utilize AWS services. Which AWS service could be used in place of the third-party software?

## CORRECT: "AWS Batch" is the correct answer.


# A Solutions Architect enabled Access Logs on an Application Load Balancer (ALB) and needs to process the log files using a hosted Hadoop service. What configuration changes and services can be leveraged to deliver this requirement?

## CORRECT: "Configure Access Logs to be delivered to S3 and use EMR for processing the log files" is the correct answer.


# A company has multiple Amazon VPCs that are peered with each other. The company would like to use a single Elastic Load Balancer (ELB) to route traffic to multiple EC2 instances in peered VPCs within the same region. How can this be achieved?

## CORRECT: "This is possible using the Network Load Balancer (NLB) and Application Load Balancer (ALB) if using IP addresses as targets" is the correct answer.


# A Solutions Architect needs to run a PowerShell script on a fleet of Amazon EC2 instances running Microsoft Windows. The instances have already been launched in an Amazon VPC. What tool can be run from the AWS Management Console that to execute the script on all target EC2 instances?

## CORRECT: "Run Command" is the correct answer.


# A company is deploying a new two-tier web application that uses EC2 web servers and a DynamoDB database backend. An Internet facing ELB distributes connections between the web servers. The Solutions Architect has created a security group for the web servers and needs to create a security group for the ELB. What rules should be added? (choose 2)

## CORRECT: "Add an Outbound rule that allows HTTP/HTTPS, and specify the destination as the web server security group" is a correct answer.
## CORRECT: "Add an Inbound rule that allows HTTP/HTTPS, and specify the source as 0.0.0.0/0" is also a correct answer.


# A Solutions Architect is launching an Amazon EC2 instance with multiple attached volumes by modifying the block device mapping. Which block device can be specified in a block device mapping to be used with an EC2 instance? (choose 2)

## CORRECT: "EBS volume" is a correct answer.
## CORRECT: "Instance store volume" is also a correct answer.


# A Solutions Architect has created a VPC and is in the process of formulating the subnet design. The VPC will be used to host a two-tier application that will include Internet facing web servers, and internal-only DB servers. Zonal redundancy is required. How many subnets are required to support this requirement?

# CORRECT: "4 subnets" is the correct answer.


# One of the departments in a company has been generating a large amount of data on Amazon S3 and costs are increasing. Data older than 90 days is rarely accessed but must be retained for several years. If this data does need to be accessed at least 24 hours notice is provided. How can a Solutions Architect optimize the costs associated with storage of this data whilst ensuring it is accessible if required?

# CORRECT: "Use S3 lifecycle policies to move data to GLACIER after 90 days" is the correct answer.


# The Solutions Architect in charge of a critical application must ensure the Amazon EC2 instances are able to be launched in another AWS Region in the event of a disaster. What steps should the Solutions Architect take? (Select TWO.)

## CORRECT: "Create AMIs of the instances and copy them to another Region" is the correct answer.
## CORRECT: "Launch instances in the second Region from the AMIs" is also a correct answer.


# An application runs on EC2 instances in a private subnet behind an Application Load Balancer in a public subnet. The application is highly available and distributed across multiple AZs. The EC2 instances must make API calls to an internet-based service. How can the Solutions Architect enable highly available internet connectivity?

# CORRECT: "Create a NAT gateway in the public subnet of each AZ. Update the route tables for each private subnet to direct internet-bound traffic to the NAT gateway" is the correct answer.


# A security officer has requested that all data associated with a specific customer is encrypted. The data resides on Elastic Block Store (EBS) volumes. Which of the following statements about using EBS encryption are correct? (choose 2)     

## CORRECT: "Data in transit between an instance and an encrypted volume is also encrypted" is the correct answer.
## CORRECT: "There is no direct way to change the encryption state of a volume" is the correct answer.


# The application development team in a company have developed a Java application and saved the source code in a .war file. They would like to run the application on AWS resources and are looking for a service that can handle the provisioning and management of the underlying resources it will run on. Which AWS service should a Solutions Architect recommend the Developers use to upload the Java source code file?

## CORRECT: "AWS Elastic Beanstalk" is the correct answer.

 
# A web application runs on a series of Amazon EC2 instances behind an Application Load Balancer (ALB). A Solutions Architect is updating the configuration with a health check and needs to select the protocol to use. What options are available? (choose 2)

## CORRECT: "HTTP" is the correct answer.
## CORRECT: "HTTPS" is the correct answer.


# An Amazon EC2 instance is generating very high packets-per-second and performance of the application stack is being impacted. A Solutions Architect needs to determine a resolution to the issue that results in improved performance. Which action should the Architect take?

## CORRECT: "Use enhanced networking" is the correct answer.


# A government agency is using CloudFront for a web application that receives personally identifiable information (PII) from citizens. What feature of CloudFront applies an extra level of encryption at CloudFront edge locations to ensure the PII data is secured end-to-end?   

## CORRECT: "Field-level encryption" is the correct answer.

 
# A company runs an application on premises that stores a large quantity of semi-structured data using key-value pairs. The application code will be migrated to AWS Lambda and a highly scalable solution is required for storing the data. Which datastore will be the best fit for these requirements?

## CORRECT: "Amazon DynamoDB" is the correct answer.


# An application makes calls to a REST API running on Amazon EC2 instances behind an Application Load Balancer (ALB). Most API calls complete quickly. However, a single endpoint is making API calls that require much longer to complete and this is introducing overall latency into the system. What steps can a Solutions Architect take to minimize the effects of the long-running API calls?

## CORRECT: "Create an Amazon SQS queue and decouple the long-running API calls" is the correct answer.


# A Solutions Architect is designing the system monitoring and deployment layers of a serverless application. The system monitoring layer will manage system visibility through recording logs and metrics and the deployment layer will deploy the application stack and manage workload changes through a release management process. The Architect needs to select the most appropriate AWS services for these functions. Which services and frameworks should be used for the system monitoring and deployment layers? (choose 2)

## CORRECT: "Use AWS SAM to package, test, and deploy the serverless application stack" is a correct answer.
## CORRECT: "Use Amazon CloudWatch for consolidating system and application logs and monitoring custom metrics" is also a correct answer.


# An Auto Scaling group of Amazon EC2 instances behind an Elastic Load Balancer (ELB) is running in an Amazon VPC. Health checks are configured on the ASG to use EC2 status checks. The ELB has determined that an EC2 instance is unhealthy and has removed it from service. A Solutions Architect noticed that the instance is still running and has not been terminated by EC2 Auto Scaling. What would be an explanation for this behavior?


## CORRECT: "The ELB health check type has not been selected for the ASG and so it is unaware that the instance has been determined to be unhealthy by the ELB and has been removed from service" is the correct answer.

# A Solutions Architect has created an AWS account and selected the Asia Pacific (Sydney) region. Within the default VPC there is a default security group. What settings are configured within this security group by default? (choose 2)


## CORRECT: "There is an inbound rule that allows all traffic from the security group itself" is a correct answer.
## CORRECT: "There is an outbound rule that allows all traffic to all addresses" is also a correct answer.


# An Amazon EBS-backed EC2 instance has been launched. A requirement has come up for some high-performance ephemeral storage. How can a Solutions Architect add a new instance store volume?

## CORRECT: "You can specify the instance store volumes for your instance only when you launch an instance" is the correct answer.


# A company runs a streaming media service and the content is stored on Amazon S3. The media catalog server pulls updated content from S3 and can issue over 1 million read operations per second for short periods. Latency must be kept under 5ms for these updates. Which solution will provide the BEST performance for the media catalog updates?


## CORRECT: "Update the application code to use an Amazon ElastiCache for Redis cluster" is the correct answer.


# A Solutions Architect has created a new Network ACL in an Amazon VPC. No rules have been created. Which of the statements below are correct regarding the default state of the Network ACL? (choose 2)

## CORRECT: "There is a default inbound rule denying all traffic" is a correct answer.
## CORRECT: "There is a default outbound rule denying all traffic" is also a correct answer.


# An Amazon DynamoDB table has a variable load, ranging from sustained heavy usage some days, to only having small spikes on others. The load is 80% read and 20% write. The provisioned throughput capacity has been configured to account for the heavy load to ensure throttling does not occur. What would be the most efficient solution to optimize cost?

## CORRECT: "Create a DynamoDB Auto Scaling scaling policy" is the correct answer.


# The database layer of an on-premises web application is being migrated to AWS. The database currently uses an in-memory cache. A Solutions Architect must deliver a solution that supports high availability and replication for the caching layer. Which service should the Solutions Architect recommend?

## CORRECT: "Amazon ElastiCache Redis" is the correct answer.


# An organization in the agriculture sector is deploying sensors and smart devices around factory plants and fields. The devices will collect information and send it to cloud applications running on AWS. Which AWS service will securely connect the devices to the cloud applications?

## CORRECT: "AWS IoT Core" is the correct answer.


# A distribution method is required for some static files. The requests will mainly be GET requests and a high volume of GETs is expected, often exceeding 2000 per second. The files are currently stored in an S3 bucket. According to AWS best practices, how can performance be optimized?

## CORRECT: "Integrate CloudFront with S3 to cache the content" is the correct answer.


# A company requires an Elastic Load Balancer (ELB) for an application they are planning to deploy on AWS. The application requires extremely high throughput and extremely low latencies. The connections will be made using the TCP protocol and the ELB must support load balancing to multiple ports on an instance. Which ELB would should the company use?

## CORRECT: "Network Load Balancer" is the correct answer. 
