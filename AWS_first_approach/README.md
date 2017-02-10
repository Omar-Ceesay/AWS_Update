<link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/css/bootstrap.min.css'><link rel='stylesheet' href='https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css'><link rel='stylesheet' href='http://bcbs-cloud-docs.s3-website-us-west-2.amazonaws.com/styles/website.css'>

# AWS First Approach

****

* AWS first approach to deployment
  * Enables us to leverage the vast infrastructure AWS instead of building infrastructure
  * Enables us to dive directly into detailed solutions instead of generic higher level solutions
  * Other deployments will be used for specific solutions. Examples:
    * Google for cloud maps services
    * Azure for Microsoft integration
    * Local data center for legacy data
* AWS first approach to tools and methodology
  * Allows us leverage AWS capabilities and flexibility
  * Enables us to minimize custom integrations
  * Tools and capabilities work together natively & maintain all native features
  * Examples: CodeCommit for Git AWS Git repos;
* “Open source” approach to AWS environments
  * Automation code, utilities, microservices, templates, should all be checked in to common CodeCommit repository
  * SDLC practices should be used for infrastructure build
* Stay as high level as possible:
  * Saves costs, let’s AWS handle details
  * Enables us to focus on members/customers instead of IT
* Infrastructure built in conjunction with Customer deliverable needs where possible
  * DevOps engineers join projects
  * Build what is needed for that project
* Serverless first approach. Serverless greatly simplifies the environment:
  * Scaling is inherent and transparent
  * Removes all complexity inherent to VMs
  * No managing and updating VM images
  * No permanent jump host needed
  * No proxy, outbound internet access issues
  * No server upgrades
  * No need to log in to servers (no SSH key rotation problem for servers)
  * Avoid cost of running idle cloud infrastructure
  * Principle: infra scripts should be also use serverless architecture
