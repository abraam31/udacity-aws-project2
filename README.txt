This is the second project in Udacity Devops Nanodegree. It consists of deploying a webapp by deploying it in private subnets, and accessing it through a loadbalancer located in the public subnet, by retrieving a code from an existing public S3 bucket and deploying it on Tomcat.

Deployment is completely automated by AWS CloudFormation through 2 stacks: 

- Network stack: Stack file cloudformation.yml and params files: cloudformation-params.json
- Computing stack: Stack file Udacityproject.yml and params file: udacityproject-params.json

Network stack exposes output to be used by the computing stack.
Computing stack exposes the public DNS name of our application loadbalancer.

You can access the application by this URL
udaci-WebAp-A1Y25IU88QKH-368181010.eu-west-1.elb.amazonaws.com
