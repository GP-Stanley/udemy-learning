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
  - [Grafana Features](#grafana-features)


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

## Grafana Features
* **Visualisation Options**: Grafana provides a wide range of visualisation options, making it **easier to map data** to suitable visualisations.
* **Alerts**: Dashboards can include **alert setups**, allowing for **easier identification** and **management of alerts**.
* **Unified View**: Grafana supports **multiple data sources** in a single dashboard, providing a unified view.
* **Community Support**: A vibrant community contributes to the development of Grafana, enhancing its features and capabilities.
* **Plugins**: Grafana supports both **official and third-party plugins**, allowing for extended functionality.
* **Collaboration**: Grafana's **single-pane view** facilitates collaboration among multiple teams by providing a unified view of data.