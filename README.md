# AWS-PROJECTS
Deploying a high-availability WordPress website with an external Amazon RDS database to Elastic Beanstalk
FIRST:  launch a DB in amazon RDS(relational database service) and enable a multi AZ environment to minimize latency spikes.
Modify the security group attached to it in order to allow inbound traffic on the appropriate port.

DOWNLOAD WORDPRESS : download the configuration files from a sample repository eg : 'wget https://github.com/aws-samples/eb-php-wordpress/releases/download/v1.1/eb-php-wordpress-v1.zip'
extract wordpress and the configuration files.

LAUNCH AN ELASTIC BEAN ENVIRONMENT:  The elastic beanstalk environment creates resources such as : EC2 instances, security groups, load balancer, S3 buckets, auto scaling groups, cloudwatch alarms, cloudformation stacks and domain name.
When you terminate your environment, Elastic Beanstalk terminates all the resources that it contains.

