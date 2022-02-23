This template deploys a Cloud9 EC2 based environment. 

By default the ownership of the Cloud9 enviroment will be the user who runs the template.

There's a small rest service that captures the IP address of the caller and uses it to update the security group of the Ec2 instance where Cloud9 is running.
The Ec2 security group update is currently hardcoded to port 8080 in the lambda function but can be easily converted into a parameter and lambda environment variable.
