# Glue_Job_Automation
This repo contains the blog posts for automation of Glue Jobs along with the SNS notifications on AWS

SNS topic to be created with Email subscriptions


![image](https://user-images.githubusercontent.com/28874545/178905147-5b2a1368-5aac-4566-bebb-7e5b00599a7e.png)

Once the SNS topic has been created, create subscriptions. Here we need to enter the email Ids of the recepients, once we do that we get a conformation message from AWS which we need to accept. Once the conformation is done, we can create rules in event brigde based on the glue job state (Succeed or Failure)

Glue Job from AWS console

![image](https://user-images.githubusercontent.com/28874545/178899483-1265f7b4-4180-4163-8f59-6402f32e8182.png)


Create a Rule in Event Bridge

<img width="652" alt="image" src="https://user-images.githubusercontent.com/28874545/178899825-45fcdf6c-dd40-4852-8a60-173d373a27a7.png">

Scroll Down to the Event Pattern Section in Step 2, Enter the Glue Job name in the Empty field Called Job Name.


![image](https://user-images.githubusercontent.com/28874545/178900169-f25bad9e-9ff3-4b45-b58a-2d56c5657f35.png)


Select the target:

Here we give SNS topic created in the first part 

![image](https://user-images.githubusercontent.com/28874545/178904610-124c56aa-192a-4271-bc70-c65bc4483420.png)


Configure the tags and save it 
