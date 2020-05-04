# How to Connect EC2 with S3 inside AWS:
>	+ By default, services of AWS can’t communicate with each other 
>	+ We have to create communication link
>	+ To create communication link between services, we have to use IAM Role service of AWS
>	+ IAM stands for Identity and Access Management
>	+ IAM Role define the set of permission for making AWS service request
>	+ Then we to create policies which is basically rules to give particular access.
>	+ Policies are written in JSON.
>	+ Policies are attached to IAM Role and IAM Role attached to Resources in our condition resources are EC2 and S3.
>   + To create IAM Role follow following steps:
>	    + Go to AWS console
>	    + Go to services
>	    + Search for IAM and click on it
>	    + Go to role in dashboard of IAM
>	    + Click on create role
>	    + Then select EC2 service and click on next permissions
>	    + You have to select policies, it’s up to you that you want policies already created by AWS or you can create your own policies.
>	    + In my case I am going with AWS’s default policies for S3
>	    + In search box search s3
>	    + Select required policies like full access, read only access, etc and then click on next tag
>	    + It is optional to give tag
>	    + Click on next i.e. review section where enter name or your IAM Role and click on create role
> + Now we have to attach our IAM Role with EC2
> + Go to EC2 dashboard and follow following steps
>	   + Click on running instance
>	   + Select instance and go to action
>	   + Instance state -> start
>	   + Instance setting -> attach/replace IAM Role
>	   + Now select your IAM Role which created recently from drop down box and hit on apply
> +	Now open your linux terminal and connect your EC2 instance using SSH
> +	Check whether communication link between EC2 and S3 establish or not 
> +	Run following command on linux terminal
**aws s3** *your_command*\
for example: **aws s3 ls** 

# How to Connect EC2 with S3 outside AWS:

> + To connect services outside AWS, You need to download AWS CLI follow following step to setup AWS CLI in your machine: 
>      + Click on this link <https://aws.amazon.com/cli/>
>      + Now download setup file according to OS of your machine
>      + After downloading run setup file
> - - -
> ![](1.jpg)
> Click on **Next**
> - - - 
> ![](2.jpg)
> Select **"I accept the terms in the License Agreement"** and click on **Next** 
> - - -
>![](3.jpg)
> Click on **Next**
> - - -
>![](4.jpg)
> Click on **Install**
> - - -
>![](5.jpg)
> Click on **Finish**
> - - -
> + Check whether AWS CLI install succefully in your machine or not:
>      + Open your command prompt
>
>![](6.jpg)
> - - -
> ![](7.jpg)
> Execute **aws --version**
> - - -
> + Check whether AWS CLI have communication link between services or not:
>      + Try to execute **aws s3 ls** command in your command prompt 
>
>      ![](8.jpg)
>
>      + As you see we have to configure our AWS CLI
> + How to Configure AWS CLI:
>   + Login to your AWS account
>   + Go to **Account Details**
> ![](9.jpg)
> Click on **Show**
>   + You will get keys related to your account copy them and find out **.aws** folder in your directory and paste it
>   + Once you have done with it, try to run **aws s3 ls**
> ![](10.jpg)
>   + Now you can access your AWS services from your machine

