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
3. 

![My Image](./images/Screenshot%202024-07-06%20135255.png)

![My Image](./images/Screenshot%202024-07-06%20135318.png)

#### Step 3: Choose EC2 Metrics

Under "Create Alarm," select "EC2" from the list of metrics.
Click on the "Per-Instance Metrics" tab.
Search and Choose your desired EC2 instance from the list.



#### Step 4: Define the Alarm Condition

Under the "Select metric" dropdown, choose "Per-Instance Metrics."
Select "CPUUtilization" from the list of metrics.
Specify the conditions for the alarm. For example, set the threshold to trigger the alarm when the CPU utilization exceeds 10% for  consecutive periods of 1 minutes.

#### Step 5: Define the Actions

Under the "Whenever this alarm state is" section, select the specific state (e.g., "In Alarm").
Choose an existing SNS topic or create a new one to receive notifications when the alarm state changes.

#### Step 6: Name and Create the Alarm

Provide a descriptive name and description for the alarm.
Click on the "Create alarm" button to finalize and create the CloudWatch alarm.

#### Step 7: Verification

Once the alarm is created, navigate to the "Alarms" section in the CloudWatch console to verify that the new alarm for CPU utilization is active.
Conclusion:
In this guide, you have learned how to create a CloudWatch alarm to monitor the CPU utilization of an EC2 instance. By setting up this alarm, you can proactively monitor the performance of your EC2 instances and take necessary actions to maintain optimal operational efficiency.

Note: Regularly review and adjust your CloudWatch alarm settings based on the specific needs and performance characteristics of your EC2 instances.
