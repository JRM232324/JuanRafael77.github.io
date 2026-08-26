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
