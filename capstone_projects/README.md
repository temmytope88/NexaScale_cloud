# Nexascale AWS Cloud Mentorship Program Capstone Projects

## 1. Monitoring and Logging with CloudWatch

   • Set up CloudWatch alarms to monitor EC2 instance CPU utilization.
   • Create custom CloudWatch metrics and dashboards.

### Introduction

Amazon CloudWatch is a monitoring and management service that provides data and actionable insights for AWS resources. This technical writing guide will illustrate the step-by-step process of creating a CloudWatch alarm to monitor CPU utilization of an EC2 instance.

### Prerequisites

1. An active AWS account.
2. Access to the AWS Management Console.
3. An existing EC2 instance for monitoring.

#### Step 1: Navigate to the CloudWatch Console

1. Log in to your AWS Management Console.
2. In the Find Services search bar, type "CloudWatch" and select the CloudWatch service.

#### Step 2: Create an Alarm

1. In the CloudWatch console, select "Alarms" from the left navigation pane.
2. Click on the "Create Alarm" button.

![My Image](./images/Screenshot%202024-07-06%20135255.png)

![My Image](./images/Screenshot%202024-07-06%20135318.png)

#### Step 3: Choose EC2 Metrics

1. Click on select metric and selct EC2 from the list of metrics.
2. Click on the "Per-Instance Metrics" tab.
3. Search and Choose your desired EC2 instance from the list using the EC2 instance id.

![My Image](./images/Screenshot%202024-07-06%20135340.png)

![My Image](./images/Screenshot%202024-07-06%20135405.png)

![My Image](./images/Screenshot%202024-07-07%20050117.png)

#### Step 4: Define the Alarm Condition

1. Select "CPUUtilization" from the list of metrics.
2. Specify the conditions for the alarm. For example, set the threshold to trigger the alarm when the CPU utilization exceeds 50% for  consecutive periods of 1 minutes.

![My Image](./images/Screenshot%202024-07-07%20050315.png)

![My Image](./images/Screenshot%202024-07-07%20050535.png)

#### Step 5: Define the Actions

1. Under the "Whenever this alarm state is" section, select the specific state (e.g., "In Alarm").
2. Choose an existing SNS topic or create a new one to receive notifications when the alarm state changes.

![My Image](./images/Screenshot%202024-07-07%20050758.png)

#### Step 6: Name and Create the Alarm

Provide a descriptive name and description for the alarm and click on next
In the preview and create page, click on the "Create alarm" button to finalize and create the CloudWatch alarm.
![My Image](./images/Screenshot%202024-07-07%20052239.png)

![alt text](<./images/Screenshot 2024-07-07 052716.png>)

#### Step 7: Test the Cloudwach alarm

1. ssh into the specific EC2 instance and install stress on it for the test.
2. Carry out the stress test using the command below. (--cpu and -timeout indicates the number of cpu and the time length of the test)

![My Image](./images/Screenshot%202024-07-06%20143325.png)

The image below shows the email sent when the alarm was triggered

![My Image](./images/Screenshot%202024-07-06%20143301.png)

## 2. How to Create a Cloudwatch Dashboard

1. Click on dashboard on the side bar.
2. Click on create dashboard and give it your desired name.
3. Click on the desired type of dashboard
4. Search for the resource e.g EC2 instance and select the desired metrics to be measured e.g CPUUtilization.

![My Image](./images/Screenshot%202024-07-07%20053602.png)

![My Image](./images/Screenshot%202024-07-07%20053639.png)

![My Image](./images/Screenshot%202024-07-07%20054139.png)
