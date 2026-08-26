---
layout: default
title: "Portfolio"
permalink: /portfolio/
---

# My Portfolio

A collection of my projects, experiments, and development work.

---

## Projects

### Wazuh SIEM & Endpoint Monitoring Homelab

A self-hosted Wazuh SIEM environment deployed using Docker on Ubuntu Server. The project involved configuring a Wazuh Manager, Indexer and Dashboard, deploying an endpoint agent, monitoring security events and testing File Integrity Monitoring.

Skills: SIEM, Wazuh, Docker, Linux, Security Monitoring, FIM, Troubleshooting

[View Wazuh Project →]({{ "/projects/wazuh/" | relative_url }})

I built and configured a self-hosting Wazuh monitoring environment to gain practical experience with tools used for Security Information and Event Management (SIEM), endpoint monitoring, the collection of logs and additional monitoring such as File Integrity Monitoring (FIM).

Overall, the project consisted of installing and deploying Wazuh through Docker onto a virtual machine hosted by Virtualbox, the virtual machine ran on Ubuntu Server version 24.04 LTS. After troubleshooting connectivity issues and a deployment onto a virtual machine without enough storage, I was able to simulate a small scale security monitoring environment, similar to what might be found within a SOC.

**Objectives:**

- Deploy a functional Wazuh SIEM environment
- Configure a Wazuh Manager, Indexer and Dashboard
- Deploy a Wazuh agent onto an Ubuntu server as an endpoint
- Establish communication between the endpoint and Wazuh Manager
- Monitor endpoint security events
- Configure and test FIM
- Understand the flow of information from endpoint to the SIEM

**Environment**

The Wazuh Server was deployed using Docker Compose on an Ubuntu server, the environment included:

- Wazuh Manager to process and analyse security events
- Wazuh Indexer to store and index security data
- Wazuh Dashboard to provide a web-based interface to analyse events
- Docker / Docker Compose which was used to deploy and manage the components above

Using the Wazuh Dashboard, it provided an interface that was used to monitor the environment from the server.

**Wazuh Agents**

Utilizing Wazuh, I created an agent called Wazuh_Agent, which then was ran on the endpoint hosted by the Ubuntu server. This agent was used to monitor system activity, collect security data and securely forward the data gathered to the Wazuh Indexer for threat detection and analysis.

The image below shows Wazuh_Manager active and functioning correctly.

![Wazuh Dashboard]({{ "/assets/homelab/images/wazuhmanager/agent.png" | relative_url }})

**File Integrity Monitoring**

Through the use of Wazuh, the server was able to monitor specific files and directories for changes through the use of the agent. This can be used to identify suspicious activity within the environment, such as unauthorised modifications to system files.

Below I used the agent created within the Wazuh Dashboard to analyze the actions carried out to create, edit then delete a file called wazuh-fim-test.txt. This was done to test the FIM.

![Wazuh FIM Showcase]({{ "/assets/homelab/images/wazuhmanager/events.png" | relative_url }})

**Vulnerability Monitoring**

As well as being able to carry out FIM operations, the dashboard allowed me to view the individual vulnerabilities within the environment, where they were then categorised into different threat levels and then allowed for further analysis and planning how to help secure the server from said vulnerabilities.

![Wazuh Vulnerability Showcase]({{ "/assets/homelab/images/wazuhmanager/vulnerabilities.png" | relative_url }})

Alongside this, Wazuh Dashboard also allowed me to inspect an inventory that contained all of the vulnerabilities, where I could freely use filters to track any specific event.

![Wazuh Inventory Showcase]({{ "/assets/homelab/images/wazuhmanager/inventory.png" | relative_url }})

**Skills Demonstrated**

- SIEM Deployment
- Wazuh Management
- Docker & Docker Compose
- Troubleshooting
- Security Event Monitoring
- Analysis of logs and information forwarded to Wazuh
- Service Management
- Security telemetry pipelines
- Incident investigation fundamentals
- Configuration management

**Conclusion**

This project gave me proper practical experience regarding how a real security monitoring environment functions, how to build it and how to troubleshoot it.

Rather than simply installing Wazuh on an existing server, I had to create the endpoint, that being the Ubuntu server virtual machine, I established manager communication, investigated logs regarding FIM while validating it as a whole as well as followed security events through the monitoring pipeline.

In conclusion, the project gave me a clearer understanding of many things regarding SIEMs, alongside how in the future I may present this information to a security analyst.

---

### Enterprise Ubuntu Home Lab

A virtualised Ubuntu Server environment designed to simulate a small business infrastructure. The project includes Docker, Nginx, Grafana, Prometheus, Portainer, UFW and Fail2Ban.

Skills: Linux Administration, Virtualisation, Docker, Networking, Monitoring, Security Hardening

[View Enterprise Home Lab →]({{ "/projects/enterprise-homelab/" | relative_url }})

The Enterprise Ubuntu Home Lab is a virtualised server that I have built through the use of Ubuntu Server 24.04 LTS within Oracle Virtualbox, this server was created to simulate the deployment and management of small business infrastructure as well as develop practical Linux skills such as system administration, networking, containerisation and automation skills inside of a realistic environment.

This server hosts multiple containerised services through the use of Docker and Docker Compose, these include nginx to carry out web hosting utilities, Grafana and Prometheus for system monitoring ability and then Portainer for overall container management. Security is then strengthened and emboldened through the use of UFW, Fail2Ban.

**Technologies used:**

- Windows OS
- Oracle Virtualbox
- Ubuntu Server 24.04 LTS
- Docker & Docker Compose
- Nginx
- Grafana
- Prometheus
- Portainer
- UFW Firewall
- Fail2Ban
- Git & Github

**Key skills Demonstrated:**

- Linux System Administration
- Virtualisation
- Docker Container Management
- Web Server Configuration
- Infrastructure Monitoring
- Network Configuration
- Server Security Hardening
- Bash Scripting & Automation

### Project Screenshots:

**Virtual Machine Setup**

![Ubuntu Server running in Virtualbox, main device connected to it]({{ "/assets/homelab/images/homeandvmdisplay.png" | relative_url }})

*Ubuntu Server 24.04 LTS running inside Oracle VirtualBox as well as a Windows machine connected to it via Ubuntu terminal.*

**Docker Container Deployment**

![Docker containers operating]({{ "/assets/homelab/images/dockerdisplay.png" | relative_url }})

*Docker containers running the deployed services.*

---

### Containers In Use

![Nginx container running]({{ "/assets/homelab/images/nginxdisplay.png" | relative_url }})
![Grafana container running]({{ "/assets/homelab/images/grafanadisplay.png" | relative_url }})
![Portainer container running]({{ "/assets/homelab/images/portainerdisplay.png" | relative_url }})
![Prometheus container running]({{ "/assets/homelab/images/prometheusdisplay.png" | relative_url }})

*Docker Containers being accessed through Firefox, displays the ability to access different services within the same server.*

## Blog

Follow my progress and read about my latest work:

[View Blog Posts]({{ "/blog/" | relative_url }})
