- [Course Overview](#course-overview)
  - [Learning Objectives](#learning-objectives)
  - [Monitoring and Alerting Services](#monitoring-and-alerting-services)
  - [Specific AWS Services](#specific-aws-services)
    - [EBS (Elastic Block Storage)](#ebs-elastic-block-storage)
    - [RDS (Relational Database Service)](#rds-relational-database-service)
    - [ELB (Elastic Load Balancer)](#elb-elastic-load-balancer)
  - [Billing and Costs](#billing-and-costs)
  - [Course Outcomes](#course-outcomes)
- [Understanding Monitoring and Alerting Services in AWS](#understanding-monitoring-and-alerting-services-in-aws)
  - [Overview](#overview)
  - [Introduction to Monitoring and Alerting](#introduction-to-monitoring-and-alerting)
    - [System Monitoring](#system-monitoring)
    - [Importance of Monitoring](#importance-of-monitoring)
  - [Monitoring vs. Alerting](#monitoring-vs-alerting)
    - [Monitoring](#monitoring)
    - [Alerting](#alerting)
  - [AWS Monitoring and Alerting Services](#aws-monitoring-and-alerting-services)
    - [CloudWatch](#cloudwatch)
    - [Simple Notification Service (SNS)](#simple-notification-service-sns)
    - [Simple Email Service (SES)](#simple-email-service-ses)
- [AWS Monitoring Overview](#aws-monitoring-overview)
  - [Overview of Monitoring and Alerting Services in AWS](#overview-of-monitoring-and-alerting-services-in-aws)
    - [AWS Management Console](#aws-management-console)
    - [Viewing AWS Services](#viewing-aws-services)
    - [CloudWatch](#cloudwatch-1)
    - [CloudWatch Service Management Console](#cloudwatch-service-management-console)
    - [Simple Notification Service (SNS)](#simple-notification-service-sns-1)
    - [SNS Dashboard](#sns-dashboard)
- [What can we Monitor on AWS?](#what-can-we-monitor-on-aws)
  - [Notes on Monitoring and Alerting in AWS](#notes-on-monitoring-and-alerting-in-aws)
    - [What to Monitor on AWS](#what-to-monitor-on-aws)
    - [Importance of Monitoring](#importance-of-monitoring-1)
    - [Alert Mechanisms](#alert-mechanisms)
    - [Monitoring Usage Charges](#monitoring-usage-charges)
    - [Custom Metrics and Log Monitoring](#custom-metrics-and-log-monitoring)
    - [CloudWatch Capabilities](#cloudwatch-capabilities)
- [AWS Metrics and CloudWatch](#aws-metrics-and-cloudwatch)
  - [Overview of Metrics in AWS](#overview-of-metrics-in-aws)
  - [Monitoring Resource Health Metrics Tab](#monitoring-resource-health-metrics-tab)
    - [Example Metrics](#example-metrics)
  - [Current Metrics in (example) Account](#current-metrics-in-example-account)
  - [Viewing Metric Details](#viewing-metric-details)
  - [Data Collection and Alerting](#data-collection-and-alerting)
- [What is AWS CloudWatch?](#what-is-aws-cloudwatch)
  - [Key features and functionalities:](#key-features-and-functionalities)
- [Introduction to AWS CloudWatch](#introduction-to-aws-cloudwatch)
  - [Overview of Metrics in AWS](#overview-of-metrics-in-aws-1)
  - [AWS S3 Overview](#aws-s3-overview)
  - [Demonstration Steps](#demonstration-steps)
    - [1. Navigate to CloudWatch Management Console](#1-navigate-to-cloudwatch-management-console)
    - [2. Setting Up an Alarm](#2-setting-up-an-alarm)
    - [3. Alarm Actions](#3-alarm-actions)
  - [Benefits of CloudWatch Alarms](#benefits-of-cloudwatch-alarms)
- [Monitoring Metrics via AWS CloudWatch](#monitoring-metrics-via-aws-cloudwatch)
  - [Visualisation of Metrics](#visualisation-of-metrics)
  - [Demonstration Steps](#demonstration-steps-1)
    - [1. CloudWatch Administration Panel](#1-cloudwatch-administration-panel)
    - [2. Insights from Visualisation](#2-insights-from-visualisation)
  - [Monitoring and Reacting to AWS Resource Changes](#monitoring-and-reacting-to-aws-resource-changes)
  - [Automation with CloudWatch Alarms](#automation-with-cloudwatch-alarms)
  - [Custom Metrics](#custom-metrics)
  - [Setting Up Alerts on Custom Metrics](#setting-up-alerts-on-custom-metrics)
- [Introduction to AWS SNS (Simple Notification Service)](#introduction-to-aws-sns-simple-notification-service)
  - [Overview](#overview-1)
  - [Key Features](#key-features)
  - [Integration with AWS Services](#integration-with-aws-services)
  - [Creating SNS Topics and Subscriptions](#creating-sns-topics-and-subscriptions)
    - [Create a Topic](#create-a-topic)
    - [Create a Subscription](#create-a-subscription)
  - [Supported Protocols](#supported-protocols)
    - [Example Use Case](#example-use-case)
  - [Benefits](#benefits)
- [Quiz](#quiz)

<br>

# Course Overview

## Learning Objectives
* AWS Overview: Introduction to AWS and its variety of services.
* Understanding cloud computing, its uses, and benefits.
* Identifying who uses cloud computing and how it helps run infrastructure.

## Monitoring and Alerting Services
* **AWS Cloud Monitoring**: Overview of monitoring and alerting services within AWS Cloud.
* **AWS CloudWatch**:
  * Detailed look at alarm and dashboard features.
  * Key metrics available for EC2 instances.

## Specific AWS Services
### EBS (Elastic Block Storage)
* Monitoring and alerting for EBS volumes.
* EBS is a block-level storage volume used with EC2 instances.

### RDS (Relational Database Service)
* Key metrics and monitoring for high availability and optimal performance.

### ELB (Elastic Load Balancer)
* Monitoring and alerting for ELB.
* ELB is a load balancer service and entry point for web-based applications.

## Billing and Costs
* Monitoring Costs: Importance of monitoring operational expenses within AWS Cloud.

## Course Outcomes
* **Cloud Computing Knowledge**: Gain a clear understanding of cloud computing and AWS services.
* **AWS Monitoring**: In-depth knowledge of AWS CloudWatch features like alarms, dashboards, and metrics.
* **Service Monitoring**: Understanding monitoring and alerting options for key AWS services (EC2, EBS, RDS, ELB, billing).
* **Optimisation and Cost Savings**: Improve AWS infrastructure management, leading to optimisation and cost savings.
* **Increased Value**: Enhance your value as a cloud expert and become more sought after.

<br> 

# Understanding Monitoring and Alerting Services in AWS

## Overview
Understand the services, techniques, and tools available for monitoring AWS cloud infrastructure.

## Introduction to Monitoring and Alerting

### System Monitoring
* **What is it?**: System monitoring is the process of keeping an eye on the resources and performance of your infrastructure.
* **Why is it important?**: It provides crucial insights into the health of your infrastructure and applications, helping you ensure everything runs smoothly.
* **Who benefits?**: Operational staff and IT administrators get continuous insights, which helps them maintain the system effectively.
* **Historical Data**: Monitoring also involves collecting historical data, which can be used to analyse past performance and make improvements.

### Importance of Monitoring
* **Support and Service**: Monitoring is necessary for providing top-quality support and service to users.
* **Actionable Insights**: It helps derive actionable intelligence, allowing you to make necessary adjustments to your infrastructure and applications.

## Monitoring vs. Alerting

### Monitoring
* **Bird's Eye View**: Monitoring gives you an overall view of the system's health.
* **Historical Data**: It generally involves analysing historical data and taking a reactive approach to issues.

### Alerting
* **Timely Information**: Alerting provides timely information when something unusual is detected.
* **Proactive Actions**: It allows operational teams to take proactive actions to prevent issues.
* **Automated Tasks**: Alerts can trigger automated tasks to handle situations, such as allocating a new EC2 instance if one goes down.

## AWS Monitoring and Alerting Services

### CloudWatch
* **Primary Service**: CloudWatch is the main monitoring service in AWS.
* **What it Monitors**: It monitors key metrics of various services like EC2 (virtual servers), Elastic Load Balancer (distributes incoming traffic), Elastic Block Store (storage volumes), and more.
* **Features**: CloudWatch collects and tracks metrics, monitors log files, sets alarms, and reacts to changes in AWS resources.
* **Types of Metrics**: Metrics can include general system metrics (e.g., CPU consumption, memory utilisation) and AWS service-specific metrics (e.g., read/write disk speed).

### Simple Notification Service (SNS)
* **Notifications and Alerts**: SNS is used to send notifications and alerts to operations teams.
* **When it Alerts**: It sends alerts when metrics fall outside of normal threshold values, helping teams respond quickly to issues.

### Simple Email Service (SES)
* **Email Notifications**: SES is another service used for sending notifications and alerts via email.


<br>

# AWS Monitoring Overview

## Overview of Monitoring and Alerting Services in AWS

### AWS Management Console
- Logged into AWS management console.
- AWS updates their user interface periodically.
- Concepts explained remain valid despite UI changes.

### Viewing AWS Services
- Click on the **Services** button on the top left.
- Categorised view of all AWS services is presented.

### CloudWatch
- Found under the **Management Tools** section.
- CloudWatch is a monitoring service for AWS cloud resources.
- Access CloudWatch Service management console.

### CloudWatch Service Management Console
- Interact with CloudWatch using:
  - AWS Command Line Interface (CLI)
  - AWS Console
  - AWS APIs with AWS SDK
- Tabs available: **Dashboard**, **Alarms**, **Events**, **Logs**, **Metrics**.
- Detailed review of these tabs in subsequent lectures.

### Simple Notification Service (SNS)
- Use the search box at the top to find services.
- Type **Simple Notification Service** or **SNS**.
- Filtered list of services matching the search string is presented.
- Click on **SNS** from the list.

### SNS Dashboard
- Amazon Simple Notification Service (SNS) is a fully managed push messaging service.
- Allows users to push text alerts or notifications.
- Detailed review of SNS in subsequent lectures.

<br>

# What can we Monitor on AWS?

## Notes on Monitoring and Alerting in AWS

### What to Monitor on AWS
- **Infrastructure and Resources**: Monitor the health of deployed resources using key metrics.
- **Example Metric**: CPU utilisation for EC2 instances is crucial for assessing instance health and utilisation.

### Importance of Monitoring
- **Proactive Actions**: Proper monitoring and alerting pipelines help avoid issues like CPU starvation, slowness, or downtime.
- **Load Management**: Allows for load distribution, application throttling, and debugging bottlenecks.
- **Security**: Helps identify unexpected loads from malicious users (e.g., during an attack).

### Alert Mechanisms
- **Timely Information**: Continuous monitoring and alert mechanisms provide timely alerts and notifications for abnormalities.

### Monitoring Usage Charges
- **Cloud Usage Costs**: Monitor and manage usage charges to avoid unexpected bills.
- **Billing Alerts**: Set up alerts for estimated charges to stay within budget limits.

### Custom Metrics and Log Monitoring
- **Custom Metrics**: Push custom metrics from applications to CloudWatch for specific monitoring needs.
- **Log Data Monitoring**: Use CloudWatch to monitor application logs and track error rates or specific terms (e.g., 404 status codes).

### CloudWatch Capabilities
- **Metric Collection**: Collects and monitors metrics from AWS resources.
- **Error Tracking**: Tracks errors in application logs and sends notifications when thresholds are exceeded.

<br>

# AWS Metrics and CloudWatch

## Overview of Metrics in AWS
- **AWS Management Console**: Navigate to the "CloudWatch" service.
- **Billing Alarms**:
  - Located in the "alarm section" under the "billing alarm" subsection.
  - Configure billing metrics to be collected.
  - Create alerts based on estimated billing charges.
    - Alerts can be pushed as notifications.

## Monitoring Resource Health Metrics Tab
  - View "resource health metrics".
  - Metrics are available based on the AWS services being consumed.
  - Each service has its own set of metrics collected and monitored by CloudWatch.

### Example Metrics
- **S3 Buckets**: Metrics available for created S3 buckets.
- **AWS RDS**: Metrics for database services.
- **AWS EC2**: Metrics for EC2 instances.

## Current Metrics in (example) Account
- **Services Consumed**: S3, CloudFront, RDS.
- **Total Metrics**: 80 metrics available.
  - CloudFront: 6 metrics.
  - RDS: 60 metrics.
  - S3: Remaining metrics.

## Viewing Metric Details
- **Metric Details**:
  - Click on "metrics" to see **data type** and **source**.
    - Example: S3 metrics list shows bucket name, storage type, and metric name.
- **Graph Rendering**:
  - Select a metric to see a graph of collected data.
  - Time frame selection available (e.g., last three hours, one week).
    - Example: CPU credit usage metric for RDS database shows data for the past week.

## Data Collection and Alerting
- **Data Collection**:
  - CloudWatch collects data over time.
    - Example: Data collected for S3 account over the past week.
- **SNS Integration**:
  - Wire up collected data with SNS for alerting functionality.
  - **SNS Dashboard**:
    - View topics, applications, and subscriptions.
    - **Create a topic**: SNS topics are communication channels for messages and notifications.
    - Create **endpoints** and **subscriptions** to deliver alert messages via the correct communication protocol.

<br>

# What is AWS CloudWatch?
* AWS CloudWatch is a monitoring service for AWS resources. 

## Key features and functionalities:

`Monitoring Service`
* CloudWatch helps you keep an eye on your **AWS resources** by **collecting and tracking metrics**.

`Log Monitoring`
* It can also **collect** and **monitor** **log files** from AWS services and custom applications running within your AWS infrastructure.

`Centralised Monitoring`
* With CloudWatch, you have a **single place** to view all your diagnostic information, making it easier for operations teams to get **actionable insights** without digging through multiple sources.

`Alarms and Notifications`
* You can set up alarms on any tracked metrics. 
* These **alarms** can **trigger notifications** via SMS or email, or even initiate automated actions.

`Automated Actions`
* Alarms can **trigger automated actions** like running custom scripts or calling APIs **to address issues proactively**. 
* This helps in resolving critical situations quickly, giving the operations team time to gather more information and make informed decisions.

> CloudWatch is your go-to tool for monitoring and managing the health and performance of your AWS resources, ensuring everything runs smoothly and efficiently.

<br>

# Introduction to AWS CloudWatch

## Overview of Metrics in AWS
* **AWS Management Console**: Navigate to the CloudWatch service.
* **S3 Metrics**: Demonstrate the ability to collect and monitor metrics related to S3 buckets.

## AWS S3 Overview
* **AWS S3**: Massively scalable storage service.
* **Buckets**: Collections in S3 similar to folders or directories on an operating system.

## Demonstration Steps
### 1. Navigate to CloudWatch Management Console
* Click on "S3 Metrics".
* Select a **metric** (e.g., total number of objects in a bucket called "templates").
* Current value: 66 objects.

### 2. Setting Up an Alarm
* **Objective**: Ensure the number of objects in the bucket does not exceed 66.
* **Action**: Delete new objects exceeding the first 66 objects.

Steps:
1. Navigate to the "alarms" tab.
2. Select "Create Alarm".
3. Choose the **metrics** for the alarm.
4. Define the alarm with a **name** and **description**.
5. Set **thresholds** (e.g., if the number of objects > 66 for X consecutive periods, trigger the alarm).

### 3. Alarm Actions
* **Notifications**: Send notifications to the operations team.

* **Automated Actions**
  * Route notifications to an AWS Lambda function to run appropriate code.
  * **Trigger autoscaling** actions to expand or shrink EC2 cluster size.
  * Call a **Lambda** function to **delete newly created objects** in the S3 bucket.

## Benefits of CloudWatch Alarms
* **Automatic Maintenance**: System maintained automatically without intervention from the operations team.
* **Real-Time Actions**: Actions are almost real-time, even during off-hours.
* **Proactive Resolution**: Immediate proactive resolution of critical situations.

<br>

# Monitoring Metrics via AWS CloudWatch

## Visualisation of Metrics
* **Graphs and Dashboards**: CloudWatch allows visualisation of collected data in easy-to-understand graphs and dashboards.
* **Multiple Metrics**: You can plot multiple metrics on a single graph to understand correlations.
* **Real-Time Updates**: Graphs can be updated in real-time for a quick overview of the system.

## Demonstration Steps
### 1. CloudWatch Administration Panel
* Navigate to the "CloudWatch metrics" section.
* Select **two different metrics** to be plotted on the same graph.
  * Example: Monitoring the number of objects in distinct S3 buckets.

### 2. Insights from Visualisation
* Compare metrics visually to infer correlations.
  * Example: The bucket "elastic beam US East one" has fewer objects compared to "CF templates".

## Monitoring and Reacting to AWS Resource Changes
* **Streaming Events**: CloudWatch provides streaming events to describe changes to AWS resources.
* **Setting Up Alerts**
  * Alerts can be triggered by changes in AWS resource usage.
    * Example: Deploying new EC2 instances and registering them with AWS Route 53 DNS service.

## Automation with CloudWatch Alarms
* **Automated Actions**
  * CloudWatch alarms can trigger AWS Lambda functions or custom AWS CLI scripts.
    * Example: Registering new EC2 instances with Route 53 automatically.

## Custom Metrics
* **Submitting Custom Metrics**
  * CloudWatch allows submission of custom metrics generated by applications.
  * Custom metrics can be monitored and alerts can be raised on these metrics.

* **Flexibility**
  * Not limited to AWS-provided metrics; can include internal custom metrics.
    * Example: Monitoring failed login attempts or the number of orders in an e-commerce store.

## Setting Up Alerts on Custom Metrics
* **Integration with CloudWatch Dashboard**
  * Custom metrics can be wired up like regular metrics.
  * Once tracked, alerting mechanisms can be set up on these metrics.

<br>

# Introduction to AWS SNS (Simple Notification Service)
## Overview
* AWS SNS is a **fast**, **flexible**, fully managed **push notification service**.
* It sends **individual messages** or **fan** out messages to a **large number of recipients**.
* **Cost-Effective**: Simple and cost-effective for sending push notifications to mobile devices, email recipients, or other distributed services.

## Key Features
* **SMS Messages**: Send SMS messages to mobile device users worldwide.
* Deliver messages to Simple Queue Service (SQS), Lambda functions, or any HTTP endpoint.
* **Pub/Sub Model**: SNS is a publish-subscribe messaging service.
  * **Publish-Subscribe**: Send a message to a topic, and all subscribed endpoints receive the message.
  * The sender does not need to send individual messages or track recipients.

## Integration with AWS Services
* CloudWatch Integration: Easily send or receive notifications between multiple services.
* Automation: Create flexible solutions for monitoring, alerting, and automation.

## Creating SNS Topics and Subscriptions
### Create a Topic
1. Navigate to the AWS console and create a **new topic**.
   * Example: Name the topic "my alerting admins" for cloud operations team notifications.
2. Specify a display name for SMS notifications.

### Create a Subscription
1. Click on "Create subscription".
2. Select the **protocol** (e.g., email) and **specify** the **endpoint** (e.g., email address).
3. Confirm the subscription via email to activate it.

## Supported Protocols
* **Email**: Basic notification protocol.
* **HTTP/HTTPS**: Invoke APIs to take various actions.
* **Amazon SQS**: Queue messages in a target queue for processing.
* **AWS Lambda**: Trigger Lambda functions for custom actions.
* **SMS**: Send SMS notifications for alarms.

### Example Use Case
* **CloudWatch Alarm Integration:**
  * Create an **alarm** in CloudWatch.
  * Configure the alarm to publish a message to an SNS topic when triggered.
    * Example: Alarm for the number of objects in an S3 bucket exceeding a threshold.
  * Receive email notifications when the alarm state changes.

## Benefits
* **Time and Energy Savings**: Simplifies the process for operations teams.
* **Real-Time Notifications**: Immediate alerts and actions without delays
* **Flexible Messaging**: Supports various protocols and integration scenarios.

<br>

# Quiz

1. Is it true that in today’s Agility driven applications backed by cloud computing monitoring alone is sufficient.
   * FALSE. It’s not sufficient. 
   * Monitoring in the IT world is very crucial; monitoring gives the Administrator continuous inside view of the health of the services being monitored. Also, Monitoring keeps track of the service performance and Historic monitoring data that can be later churned to produce insights on the application availability.

2. How many services are responsible for monitoring and alerting within AWS ecosystem?
   * Multiple Services. 
   * Monitoring and alerting mechanism on AWS is covered by multiple services. Besides monitoring, an Alerting mechanism is also needed so as to alert the admin about any issues with the service so that they can be rectified. AWS CloudWatch, AWS SNS etc. play a crucial role in making it all work – but a lot of other services work in conjunction with CloudWatch and SNS to collect and monitor the metrics.

3. AWS CloudWatch is the de-facto monitoring service on AWS which monitors key metrics of services like:
   * AWS EC2.
   * Elastic Block Store.
   * Eastic Load balancer.

4. _______________ is a monitoring service for AWS cloud resources and the applications you run on AWS.
   * Amazon CloudWatch is a monitoring service for AWS cloud resources and the applications you run on AWS.