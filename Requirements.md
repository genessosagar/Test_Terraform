- RDS - Primary with read replica (Multi-AZ)
- Autoscaling Groups and Launch Configuration
- Load Balancers one for Web servers and another for app servers
- Two EC2 instances for app servers
- Two EC2 instances for web servers
- Security Groups for each resource

Webapp stack - App review (MUST READ)
Code for this section is at https://github.com/cloudopsacademy/Terraformcourse . Please download the code and run it yourself. Subfolders for VPC , RDS modules exist.

Step by step method :

1) You can practise individual modules - VPC , RDS 

2) Once you are comfortable with individual modules you can launch the complete webapp

NOTE : If you run into any issues contact us at awsdatabaseguru@gmail.com

App overview :

Create a VPC

Create a Public subnet

Create a Private Subnet

Create separate security Groups for web servers, application servers, load balancers and RDS

Create a Application load balancer for web servers

Create target groups for ALB  and add instances to that group

Creating a autoscaling group of instances for web servers [linux based either ubuntu or                         Redhat ]

Launch the web servers in Public Sunet

Create a Application load balancer for Application servers

Create target groups for ALB and add instances to that group

Creating a autoscaling group of instances for Application servers [Linux based either ubuntu or Redhat]

Launch the Application servers in Private Subnet

Create a RDS  with replication feature connected to application servers

For Demo purposes  we will :

use nginx on Web Servers

Use Apache on Application Servers

