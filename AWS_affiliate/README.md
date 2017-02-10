<link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/css/bootstrap.min.css'><link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css'><link rel='stylesheet' href='http://bcbs-cloud-docs.s3-website-us-west-2.amazonaws.com/styles/website.css'>

# AWS Affiliate Accounts

****

* BlueCross Affiliate accounts are designed to provide a fully infrastructure space for affiliates that are supported by BlueCross IT. Examples:
  * Stella (Stella content sites)
  * BlueCross “New IT” applications (e.g. BlueRide)
  * IoT Exec Support Button
  * Alexa IT Support Alexa Skill->ServiceNow
  * Other affiliates or external customers
* Automation (Cloud Formations) to build VPC
  * Inbound and outbound traffic controlled
  * Outbound Internet access via NAT Gateway
  * Inbound only through ELBs, CloudFront, API Gateway, S3, or jump host (only for accounts with VMs) (80:443)
  * Services Accessed over public Internet and API Gateway
* Automation (Cloud Formations) to build consistent Docker ECS environment for each affiliate
  * Automation for Docker build, deploy, container scanning
* Each Production Account has tools provisioned for CI/CD:
  * Serverless & Docker/ECS supported
  * Centrally managed
  * CodeCommit, CodePipeline, CodeBuild
* Communication with BlueCross Utility accounts for
  * Monitoring
  * Logging
  * Access & Authorization
  * Centralized Billing
  * Security Scanning
45
