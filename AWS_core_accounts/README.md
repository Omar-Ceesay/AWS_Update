<link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/css/bootstrap.min.css'><link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css'><link rel='stylesheet' href='http://bcbs-cloud-docs.s3-website-us-west-2.amazonaws.com/styles/website.css'>

# AWS Core Accounts

****

* Serves as a bridge between AWS and BlueCross internal network
  * VPNs in place for each environment
* Provide DNS hosting for BCBS
* Future host 3rd party AWS deployed BCBS tools
  * Hipchat, Jira, etc.
* Host Lambda based Microservices to support automation of:
  * New AWS accounts
  * New applications
  * IAM add/update/remove (IAM changes likely require approval in ServiceNow and can trigger Lambda from there)
  * DNS updates
  * Provide AWS Microservice Connectivity
  * Automate provisioning of CICD projects
* Provide centralized management of  AWS accounts
  * Consolidated billing for all AWS accounts
  * AWS “Organizations” for centralized authentication and authorization
* Role and user access integration with ServiceNow
* Incident Management integration
  * Key events to create ServiceNow incidents
* Service Catalog integration
* Provide affiliate accounts approach for:
  * Monitoring
  * Logging (CloudTrail data sent to Qradar)
  * Access & Authorization
  * Centralized Billing
  * Security Scanning
* Host repositories for code and images:
  * Source code
  * NPM modules (Node.js)
  * Docker image (AWS ECR)
