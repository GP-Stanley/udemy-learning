- [What is Prometheus, Features of Grafana, Prometheus Setup on AWS](#what-is-prometheus-features-of-grafana-prometheus-setup-on-aws)
  - [What is Prometheus?](#what-is-prometheus)
    - [How it works](#how-it-works)
  - [Why Use Prometheus?](#why-use-prometheus)
  - [How Does It Help?](#how-does-it-help)
  - [Storage and Retention in Prometheus](#storage-and-retention-in-prometheus)
  - [AWS Free Tier Account and Local Setup](#aws-free-tier-account-and-local-setup)
  - [Prometheus as a Backend for Grafana](#prometheus-as-a-backend-for-grafana)

<br>

# What is Prometheus, Features of Grafana, Prometheus Setup on AWS

## What is Prometheus?
Prometheus is a powerful tool used for **monitoring** and **alerting**. Think of it as a smart system that keeps an eye on your computer programs and servers to make sure everything is running smoothly. 

### How it works
`Data Collection`
* Prometheus **collects data** from various sources, like your applications and servers. 
* This data includes things like CPU usage, memory usage, and other important metrics.

`Storage`
* It **stores** this data in a special **database** **designed** for **time-series data**. 
* This means it can keep track of how these metrics change over time.

`Querying`
* You can **ask** Prometheus **questions** **about the data** it has collected. 
  * For example, you can ask it to show you the CPU usage of a server over the past week.

`Alerting`
* Prometheus can also **send alerts** if something goes wrong. 
  * For instance, if a server's CPU usage gets too high, it can notify you so you can take action.

## Why Use Prometheus?
* **Open Source**: It's free to use and has a large community of users and developers who contribute to its improvement.
* **Scalable**: It can handle a lot of data, making it suitable for both small and large systems.
* **Flexible**: You can customise it to monitor almost anything you want.

## How Does It Help?
* Imagine you have a website, and you want to make sure it's always up and running. 
* Prometheus can **monitor your website's performance** and **alert** you if there's a **problem**, like if the website becomes slow or goes down. 
* This way, you can **quickly fix issues** before they affect your users.

> Prometheus is like a vigilant guardian for your computer systems, helping you keep everything running smoothly and alerting you when something needs your attention.

## Storage and Retention in Prometheus
* Prometheus offers a default **storage retention** of 15 days.
* **Extended Retention**: For data older than 15 days, additional configuration is required to extend retention.

## AWS Free Tier Account and Local Setup
* **AWS Free Tier**: Participants are encouraged to create an AWS free tier account for hands-on practice.
* **Local Setup**: Grafana and Prometheus can be **set up locally** for those who prefer not to use AWS.

## Prometheus as a Backend for Grafana
* **Functionality**: Prometheus acts as a backend for Grafana, **collecting** and **storing metrics**.
* **Discovery Engine**: Prometheus uses a **discovery engine** to **scrape metrics from source systems**.
* **Configuration**: **Targets are defined** in the Prometheus configuration file (prometheus.yml).
* **Exporters**: Specialised utilities (exporters) are deployed on source systems to collect metrics.
* **Integration**: Prometheus **integrates with Grafana** to provide **data for visualisation**.

