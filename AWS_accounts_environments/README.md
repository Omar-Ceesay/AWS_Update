<link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/css/bootstrap.min.css'><link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css'><link rel='stylesheet' href='http://bcbs-cloud-docs.s3-website-us-west-2.amazonaws.com/styles/website.css'>

# Accounts/Environments Approach

****

#### Distinct AWS accounts to isolate companies & environments
* Dev environments can be used for experimentation, be easily recreated using template automation
* Staging should prove deployment & maintenance automation and be production bound
* Production have little-to-no manual intervention  

#### PHI data to only be stored and manipulated in PHI designated AWS accounts
* AWS services are used based on PHI certification. These tend to be dedicated instances and higher cost
* Non-PHI services can be leveraged for designated activities as long as they are used in approved way  

#### Separate accounts enables isolation
* Enables freedom in dev accounts – can be built & rebuilt by automation
* Maintains security, isolation, automation for higher accounts
* Truly isolates separate companies
* Many AWS services (such as IAM) span account  
* Consolidated Billing and AWS Organizations used for common administration of multiple accounts  

#### “Walled garden” approach to AWS access
* Provide direct access to AWS console and APIs based on role and need
* **Example roles:**
  * Read-only
  * Developer (Git push)
  * DevOps Engineer
  * Billing Administrator
  * Administrator
