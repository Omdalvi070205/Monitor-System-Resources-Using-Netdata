# INTERNSHIP - TASK 7: Netdata Monitoring
### Objective
The objective of this task was to install and use Netdata, a free and open-source monitoring tool, to visualize system and application performance metrics. The key deliverables included a screenshot of the Netdata dashboard with running metrics.

### Tools Used
#### Netdata: The core tool for real-time performance monitoring.

#### Docker: Used to run Netdata as a lightweight container.

### Steps Taken to Complete the Task
#### Launched Netdata: Used the provided Docker command to launch the Netdata container.

##### docker run -d --name netdata -p 19999:19999 netdata/netdata

##### Accessed the Dashboard: Navigated to http://localhost:19999 in a web browser to view the Netdata dashboard.

Explored Metrics: Examined the real-time charts and panels for various system metrics, including CPU, memory, disk I/O, and Docker container performance. I also explored the alerts feature to understand its alerting capabilities.

Captured Screenshot: A screenshot of the running Netdata dashboard was captured to serve as a deliverable for the task.

### Deliverables
Screenshot: A screenshot of the Netdata dashboard showcasing system metrics.

README.md: This file, documenting the process and steps followed.

#### Interview Questions & Answers
Based on the task and my exploration of Netdata, I have prepared answers for the interview questions provided in the task document.

#### What does Netdata monitor?
Netdata monitors a wide range of metrics, including CPU utilization, memory usage, disk I/O, network traffic, system processes, and application-specific metrics for services like web servers and databases. It can also automatically discover and monitor Docker containers.

#### How do you view real-time metrics?
Real-time metrics are viewed through the web dashboard, which is accessible by navigating to http://localhost:19999 (or the host's IP address and port). The dashboard provides interactive charts that update every second.

#### How is Netdata different from Prometheus?
Netdata is designed for real-time, per-second monitoring on a single server, making it ideal for immediate troubleshooting. Prometheus, on the other hand, is a more powerful and complex system designed for long-term data storage and large-scale, distributed monitoring. Netdata is push-based (collects metrics locally and pushes them to the dashboard), while Prometheus is pull-based (pulls metrics from configured endpoints).

#### What is a collector?
A collector in Netdata is a component responsible for gathering metrics from a specific source, such as the operating system kernel, a database, or a web server. Netdata has hundreds of collectors for various applications and services, making it highly versatile.

#### What are some performance KPIs to watch?
Key performance indicators (KPIs) to watch include:

###### CPU Utilization: High usage could indicate a CPU-bound process.

###### Memory Usage: High memory usage and swap activity could point to a memory leak or an application needing more resources.

###### Disk I/O: High disk I/O wait times could indicate a bottleneck in disk performance.

###### Network Throughput: Monitoring network traffic helps identify potential bottlenecks or unusual activity.

###### System Load: The system load average gives a general idea of the system's workload over time.

