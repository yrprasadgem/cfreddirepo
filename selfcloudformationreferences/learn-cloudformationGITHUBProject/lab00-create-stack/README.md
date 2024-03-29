# Lab 0: Create a CloudFormation stack

Create a CloudFormation stack based on an existing template.

## Overview
1. Create a CloudFormation stack based on an existing template.

## Instructions
1. Open [CloudFormation](https://console.aws.amazon.com/cloudformation) in AWS Management Console.
1. Click **Create Stack** button.
1. Select **Upload a template to Amazon S3**.
1. Choose file `learn-cloudformation/lab0-create-stack/demo.yaml`.
1. Click **Next** button.
1. Insert `lab0-$username`as stack name. Replace `$username`with your username (e.g. lab0-awittig).
1. Select a random subnet and the only available VPC as **Parameters**.
1. Click **Next** button.
1. Skip next step by clicking on **Next** button.
1. Review your input and click **Create** button.
1. Wait until your stack reaches status **CREATE_COMPLETE**.
1. Select your stack by clicking on row of the table.
1. Switch to the **Outputs** tab.
1. Search for **HelloWorldURL** and click on the URL.
1. A website showing `Hello World!` should appear.
1. Select your stack by clicking on row of the table again.
1. Select **Delete Stack** from the **Actions** menu.
1. Confirm the deletion of your stack.
1. Congratulations! You are done with the lab!

################################################
REDDI PRASAD EXPERIENCE
##################################################
I HAVE CREATED THE STACK WITH OUT DEFAULT VPC AND SUBNETS  ---> IT HAS FAILED SAYING NO DEFAULT VPCs FOUND.
NOTE: New feature from the AWS they have added an option to delete/create the default VPC and related stuff like subnets etc...
So, I have created the default VPC and created the stack again it worked well.

just choose options from drop down options provided in the CF stack. if we chose private subnet the outputs tab shows the private IP
here you cant access the HELLO world on the browser

So, "update" feature with the "use current template" --> change subnet from drop down ( means we are updating the stack with different parameters) 
private to public --> click next --> click "update stack"

thats all about it now ---> check outputs and click on the IP --> in the browser we can see HELLO WORLD 

######################################################## 
