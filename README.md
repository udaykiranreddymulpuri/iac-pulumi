```Infrastructure Management with AWS and Pulumi```

```AWS CLI Configuration```

Install and configure the AWS CLI using the following commands:

aws configure --profile dev
aws configure --profile demo

```Pulumi Deployment Commands```

* Deploy the Project:
    * pulumi up

*	Switch Between Stacks:
     * pulumi select stack dev/demo

*	Initialize a New Stack:
    * pulumi stack init example

*	Destroy the Project:
    * pulumi destroy

*	Refresh the Infrastructure State:
    * pulumi refresh


```AWS Infrastructure Components```

*	Virtual Private Cloud (VPC)
    *	Created a VPC with a specified CIDR block.

*	Internet Gateway
    *	Created and attached an Internet Gateway to the VPC.

*	Availability Zones
    * Queried and obtained the first three availability zones.

*	Subnets
    *	Created public and private subnets in each availability zone.
    *	Associated subnets with corresponding route tables.

*	Route Tables
    *	Created and associated public and private route tables with the relevant subnets.

*	Security Groups
    *	Created security groups for the load balancer, EC2 instances, and RDS instance.

*	EC2 Instances
    *	Created and configured EC2 instances with the necessary security groups and IAM roles.

*	RDS (Relational Database Service)
    *	Deployed a MySQL RDS instance with specified configurations.

*	IAM (Identity and Access Management)
    *	Created an IAM role with policies for EC2 instances, and attached policies for CloudWatch and S3.

*	Load Balancer
    *	Created an Application Load Balancer with specified configurations, including listeners and target groups.

*	Auto Scaling
    *	Set up an Auto Scaling Group with scaling policies and CloudWatch alarms.

*	AWS Lambda
    *	Created an IAM role and attached necessary policies for the Lambda function.
    *	Defined and deployed an AWS Lambda function with dependencies on an S3 bucket.

*	SNS (Simple Notification Service)
    *	Created an SNS topic and subscription for the Lambda function.

*	AWS CloudWatch Alarms
    *	Configured CloudWatch alarms for scaling based on CPU utilization.

*	Route53
    *	Created a Route53 record for the load balancer.

*	AWS DynamoDB
    *	Set up a DynamoDB table with specified attributes and global secondary indexes.
    *	Configured an IAM policy for DynamoDB access and attached it to the Lambda execution role.

*	AWS S3
    *	Created an S3 bucket named "pranav-bucket-1" with private ACL settings.


```Google Cloud Platform (GCP) Resources```
*	Cloud Storage (GCS)
    *	Created a GCS bucket named "csye6225_demo_gcs_bucket" with versioning enabled.
*	GCP IAM
    *	Created a service account with necessary permissions and associated it with the GCS bucket.

*	GCP IAM Policy
    *	Attached a custom IAM policy to the Lambda execution role for GCS access.

