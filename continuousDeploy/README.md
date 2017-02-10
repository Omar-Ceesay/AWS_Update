<link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/css/bootstrap.min.css'><link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css'><link rel='stylesheet' href='http://bcbs-cloud-docs.s3-website-us-west-2.amazonaws.com/styles/website.css'>

# Continuous Deploy & Continuous Integration Process

****

### We need to define and automate the process for an AWS focused CICD process
* Leverages AWS native (serverless) CICD tools: CodeCommit, CodePipeline, CodeBuild
* Needs to include automated unit testing, automated UI testing, automated service testing
* Docker and Lambda application architectures
* Needs to include code scanning
* For container based applications:
  * For container based applications, needs to scan with Twistlock
  * Needs to commit images to AWS ECR
* Automation for code, scripts, configurations to go through accounts/environments:
  * Dev->Staging->Production
  * App developers should be able to trigger CICD from Git Push
  * Production and possibly staging changes should trigger a call to ServiceNow to record the Change (if this is required)
* Need flexibility enable anyone to contribute to, improve, or extend CICD process for unique needs  

<img src="../pictures/AWS_tools.JPG"></img>
