- [Introduction to Grafana](#introduction-to-grafana)
  - [What is Grafana?](#what-is-grafana)
  - [Why Use Grafana?](#why-use-grafana)
- [Types of Grafana](#types-of-grafana)
  - [Grafana Open Source](#grafana-open-source)
  - [Grafana Cloud](#grafana-cloud)
  - [Grafana Enterprise](#grafana-enterprise)
  - [Grafana Enterprise Logs](#grafana-enterprise-logs)
  - [Choosing the Right Grafana Version](#choosing-the-right-grafana-version)
  - [Features and Versions](#features-and-versions)
  - [Prometheus as a Backend for Grafana](#prometheus-as-a-backend-for-grafana)
- [Setting Up Grafana with Docker: A Step-by-Step Guide](#setting-up-grafana-with-docker-a-step-by-step-guide)
  - [Grafana Installation](#grafana-installation)
- [Grafana Documentation Link](#grafana-documentation-link)
- [For an AWS EC2 Instance](#for-an-aws-ec2-instance)
  - [Step 1: Install Docker](#step-1-install-docker)
  - [Step 2: Pull the Grafana Docker Image](#step-2-pull-the-grafana-docker-image)
  - [Step 3: Run the Grafana Container](#step-3-run-the-grafana-container)
  - [Stop the Grafana container](#stop-the-grafana-container)
  - [Step 4: Access Grafana](#step-4-access-grafana)
  - [Step 5: Configure Security Group (if using AWS)](#step-5-configure-security-group-if-using-aws)
- [Go to Grafana Website](#go-to-grafana-website)
  - [Step 6: Change Default Password](#step-6-change-default-password)
  - [Step 7: Add Data Sources](#step-7-add-data-sources)
  - [Step 8: Create Dashboards](#step-8-create-dashboards)

<br>

# Introduction to Grafana

## What is Grafana?
* Grafana is a powerful tool that helps you **visualise data**. 
* A multi-pltform open source analytics and interactive visualisation web application. 
  * It provides: charts, graphs, and alerts. 

> Think of it as a dashboard for all your important information. 

Here’s how it works:
`Data Visualisation`
* Grafana takes data from various sources and turns it into **easy-to-understand** **charts**, **graphs**, and **dashboards**. 
* This makes it simple to see how things are performing at a glance.

`Integration`
* It works with many different data sources like Prometheus, CloudWatch, InfluxDB, and SQL Server. 
* This means you can **pull in data** from almost anywhere.

`User-Friendly Interface`
* Grafana is designed to be **easy to use**. 
* You don’t need to be a tech expert to create beautiful, informative dashboards.

`Customisable Dashboards`
* You can **create your own dashboards** or use **pre-made templates**. 
* This allows you to display the data that matters most to you in a way that makes sense.

`Alerts and Notifications`
* Grafana can send you **alerts** when something important happens. 
  * For example, if a server is down or if there’s a spike in traffic, you’ll get notified right away.

## Why Use Grafana?
* **Better Decision Making**: By visualising your data, you can make better, more **informed decisions**.
* **Quick Insights**: Instantly see the **status** of your **systems and applications**.
* **Flexibility**: Customise your dashboards to fit your specific needs.

> Grafana is like a control center for your data, helping you keep track of everything in one place with clear and insightful visuals.

<br>

# Types of Grafana

## Grafana Open Source
* The **free** and **open-source** version of Grafana.
* **Features**: Basic features for data visualisation, dashboard creation, and alerting.
* **Use Case**: Ideal for **individuals** or **small teams** who need powerful visualisation tools without cost.

## Grafana Cloud
* A **fully managed** Grafana **service** hosted by Grafana Labs.
* **Features**: Includes advanced features like **enhanced security**, **scalability**, and **integrations** with **other cloud services**.
* **Use Case**: Suitable for organisations that prefer a managed service to avoid the overhead of maintaining their own Grafana instance.

## Grafana Enterprise
* A premium version of Grafana with **additional features and support**.
* **Features**: Includes advanced data source integrations, enterprise plugins, enhanced security, and dedicated support.
* **Use Case**: Designed for large organisations that require advanced features, support, and scalability.

## Grafana Enterprise Logs
* A specialised version focused on **log management**.
* **Features**: Provides powerful log aggregation, querying, and visualisation capabilities.
* **Use Case**: Ideal for organisations that need to manage and analyse large volumes of log data.

<br>

## Choosing the Right Grafana Version
* **Evaluation and Testing**: Organisations often start with the open-source version for initial development and testing.
* **Governance and Security**: For critical infrastructure and governance requirements, organisations may choose Grafana Enterprise or SaaS.

## Features and Versions
* **Alert Management**: Advanced alert management features in versions 9.0 and above.
* **Current Usage**: Most organisations use versions 9 or 10, with discussions about version 11.
* **UI Changes**: Minor UI changes between versions, but core features remain similar.

## Prometheus as a Backend for Grafana
* **Functionality**: Prometheus acts as a backend for Grafana, **collecting** and **storing metrics**.
* **Discovery Engine**: Prometheus uses a **discovery engine** to **scrape metrics from source systems**.
* **Configuration**: **Targets are defined** in the Prometheus configuration file (prometheus.yml).
* **Exporters**: Specialised utilities (exporters) are deployed on source systems to collect metrics.
* **Integration**: Prometheus **integrates with Grafana** to provide **data for visualisation**.

<br>

# Setting Up Grafana with Docker: A Step-by-Step Guide 

## Grafana Installation
* **AWS Free Tier Account**: Participants are encouraged to create an AWS free tier account for hands-on practice.
* **Dockerised Installation**: Demonstration of Dockerised Grafana installation using AWS EC2 instances.
* **Instance Setup**: Steps to launch an EC2 instance and set up Grafana.

# Grafana Documentation Link
Source: https://grafana.com/docs/grafana/latest/ 

# For an AWS EC2 Instance

## Step 1: Install Docker
1. Update Package List: `sudo apt-get update`
2. Install Docker: `sudo apt-get install docker.io`
3. Start Docker Service: b`sudo systemctl start docker`
4. Enable Docker to Start at Boot: `sudo systemctl enable docker`

## Step 2: Pull the Grafana Docker Image
Pull the Latest Grafana Image:  `sudo docker pull grafana/grafana`

## Step 3: Run the Grafana Container
Run the Container:`docker run -d -p 3000:3000 --name=grafana grafana/grafana-enterprise`

* `docker run` is a Docker CLI command that runs a new container from an image
* `-d` (--detach) runs the container in the background
* `-p <host-port>:<container-port>` (--publish) publish a container’s port(s) to the host, allowing you to reach the container’s port via a host port. 
  * In this case, we can reach the container’s port 3000 via the host’s port `3000`.
* `--name` assign a logical name to the container (e.g. grafana). This allows you to refer to the container by name instead of by ID.
* `grafana/grafana-enterprise` is the image to run

## Stop the Grafana container
To stop the Grafana container, run the following command:
```bash
# The `docker ps` command shows the processes running in Docker
docker ps

# This will display a list of containers that looks like the following:
CONTAINER ID   IMAGE  COMMAND   CREATED  STATUS   PORTS    NAMES
cd48d3994968   grafana/grafana-enterprise   "/run.sh"   8 seconds ago   Up 7 seconds   0.0.0.0:3000->3000/tcp   grafana

# To stop the grafana container run the command
# docker stop CONTAINER-ID or use
# docker stop NAME, which is `grafana` as previously defined
docker stop grafana
```


## Step 4: Access Grafana
1. Find the Public IP of Your Instance:
   * If you're using a cloud service like AWS, find the public IP address of your instance.

2. Open Grafana in Your Browser:
   * Go to http://<public-ip>:3000
   * The default username and password are both **admin**.

## Step 5: Configure Security Group (if using AWS)
Open Security Group Settings:
1. Go to the AWS Management Console.
2. Navigate to `EC2 > Instances > Select your instance > Security > Security Groups`.

**Edit Inbound Rules:**
1. Add a rule to allow traffic on port 3000.
   * Type: Custom TCP
   * Port Range: 3000
   * Source: Anywhere (0.0.0.0/0)

# Go to Grafana Website
## Step 6: Change Default Password
**Login to Grafana:**
* Use the default credentials (admin/admin).

**Change Password:**
* Follow the prompt to change the default password.

## Step 7: Add Data Sources
Navigate to Data Sources:
1. Click on the gear icon (⚙️) on the left sidebar.
2. Select "Data Sources".

Add a New Data Source:
1. Click "Add data source".
2. Select the type of data source you want to add (e.g., Prometheus, InfluxDB).
3. Configure the data source settings and save.

## Step 8: Create Dashboards
Create a New Dashboard:
1. Click on the "+" icon on the left sidebar.
2. Select "Dashboard" > "New Dashboard".

Add Panels:
1. Click "Add new panel".
2. Configure the panel settings and select the data source.
3. Save the dashboard.

<br> 

