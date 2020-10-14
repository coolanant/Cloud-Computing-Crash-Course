# Cloud-Computing-Crash-Course (AWS)

### Advantages
1. Cost Efficient (Pay for what you use)
2. Agile & Speed
3. Ability to scale up and down 
4. Stop guessing capacity
5. Go Global in minutes
6. Every service offers API

### Types of Cloud Deployment Models
1. Private (More Secure)
2. Public (Elastic Scaling)
3. Hybrid (Seamless)

### Types of Cloud
1. SaaS (Software) - Web Browser - Salesforce
2. IaaS (Infrasturcture as a Service) - Data Centers - AWS
3. PaaS (Platform) - Deployment - Heroku 
(AWS is all 3 of them)

## AWS Compute
- EC2 - virtual servers
- lambda - serverless
- ECS, EKS, Fargate - docker oon EC2 
_____________________________________________________________________________
### 1. EC2
- Elastic Compute Cloud
- Virtual Machine
- Diff options(OS, disk management, hardware configuartion, processor, memory RAM, hard disk, Graphics etc..)
-  Instance sizing(RAM), Instance Types(Processor), OS

### Terminology/Services
- **AMI(Amazon Machine Images)** - snapshot of virtual machine configuration 
- **Instances** are created which can be started or stopped 
- **(VPC) Virtual Private Cloud**
- **Elastic Block Store (EBS)** provides persistent block level *storage volumes* for use with Amazon EC2 instances 
- **S3 Bucket** 
- Security Groups - port number, firewall,
Web - 0.0.0.0/0 (all), App - Web, DB - App

> connection to a linux machine should be done through SSH (Secure Shell) (port 22)
> If you are on MAc, linux directly use, once instance is created
On windows you need SSH Client - putty
> convert *pem* Key to *ppk* using *putty gen*
> putty - host ip 
> SSH> Auth
> User - linux - ec2-user, windows-administrator, ubuntu
> Run Linux commands - ls, pwd, 
> Installing Apache server -`sudo yum install httpd`
> `sudo service httpd start`
> `sudo service httpd status`
> open public IP
> cd var/www/html
> sudo vim index.html
> esc :w :q

______________________________________________________________________

Let say 1 Ec2 instance is not enough for your work load
### Auto Scaling
- no additional charge
- Launch config(new server config), Auto Scaling Group(min, max, desired capacity), Scaling Plan
__________________________________________________________________

### 2. Elastic BeanStalk
