# AWS-PROJECTS
Deploying a high-availability WordPress website with an external Amazon RDS database to Elastic Beanstalk
FIRST:  launch a DB in amazon RDS(relational database service) and enable a multi AZ environment to minimize latency spikes.
Modify the security group attached to it in order to allow inbound traffic on the appropriate port.

DOWNLOAD WORDPRESS : download the configuration files from a sample repository eg : 'wget https://github.com/aws-samples/eb-php-wordpress/releases/download/v1.1/eb-php-wordpress-v1.zip'
extract wordpress and the configuration files.

LAUNCH AN ELASTIC BEAN ENVIRONMENT:  The elastic beanstalk environment creates resources such as : EC2 instances, security groups, load balancer, S3 buckets, auto scaling groups, cloudwatch alarms, cloudformation stacks and domain name.
When you terminate your environment, Elastic Beanstalk terminates all the resources that it contains.

CONFIGURE SECURITY GROUPS AND ENVIRONMENT PROPERTIES: This step ensures Elastic Beanstalk reprovisions all instances in your environment with the additional security group attached.
Add a security group to your environment using the Elastic Beanstalk console in the environments nagivation pane; choose configuration and edit to add an EC2 security group.
To configure the environment properties edit the environment properties under configuration, to reflect RDS port, name, password etc

CONFIGURE AND DEPLOY APPLICATION: go to elastic beanstalk; environment ; choose the environment created then select upload and deploy. select the files we downloaded earlier and deploy them.
#ERROR Application deployment failed at 2023-09-06T14:43:06Z with exit status 1 and error: Engine execution has encountered an error.
Incorrect application version "Wordpress-version-1" (deployment 4). Expected version "Sample" (deployment 3).




