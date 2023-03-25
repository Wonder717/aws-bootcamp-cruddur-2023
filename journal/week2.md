# Week 2 — Distributed Tracing

This week’s focus was on observability. So to kickstart my journal of what I got done, I will like to spell out 3 terms that are prevalent in this  README file and particularly on observability. They are the 3 pillars of observability. Namely: logs, traces & metrics.

To begin with, I completed the required tasks in the Todo checklist and implemented the various observability tools discussed this week in my project source code. I also looked into other third party tools that are quite standardised in the cloud industry for observability. These tools are Prometheus and Grafana. I also learnt about how to trigger anomalies in cloud systems to test the efficacy of these monitoring tools. Load Testing and Chaos Engineering are two approaches to execute the intentional effect of load testing and simulating fault injection in a workload. 

I wrote some short notes on Prometheus and Grafana as outlined below.

**AUTOMATED MONITORING USING PROMETHEUS**

Prometheus is a DevOps tool used for monitoring. It is an open source tool and is used in the monitoring and alerting of the performance of systems. It’s used to store all these metrics and data in a central database . It can be used to scrape systems to collect data. Thus, it is essentially a central system/server to view, collect and aggregate the monitoring of your applications and servers. 

Grafana offers visualisation to query the metrics collected and stored by Prometheus. It uses the query language promQL.

Two monitoring techniques are logs 🪵 & metrics 📊 

Logs are outputs and events of records written to files. 

Metrics are more of thresholds, numbers and statistics. 
 


A Prometheus server has 3 components. These are:

- DATA RETRIEVAL WORKER [Pulls metrics data]/Retrieval 
- TIME SERIES DATABASE [ stores metrics data]/Storage
- HTTP SERVER [ Accepts PromQL queries]/Http 


**Querying Prometheus**

Example Queries:

http_requests_total{status!~"4..") ==  [  • Query all HTTP status codes except 4xx ones ]

rate(http_requests_total [5m]) [30m: ] == (Returns the 5-minute rate of the http_requests_total metric for the past 30mins )


Grafana Uses PromOL in the background

**Prometheus with Docker and Kubernetes**

-  Fully compatible
-  Prometheus components available as Docker image
-  Easily to be deployed in Container Environments like Kubernetes.   
- Monitoring of K8s Cluster Node Resources out-of-the box!
