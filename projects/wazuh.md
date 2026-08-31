
---
layout: project
title: "Wazuh SIEM & Endpoint Monitoring Homelab"
permalink: /projects/wazuh/
---
<p class="project-label">03 · SIEM · Docker · Linux · Security Monitoring</p>

<h1>Wazuh SIEM &amp; Endpoint Monitoring Homelab</h1>

<p>I built and configured a self-hosting Wazuh monitoring environment to gain practical experience with tools used for Security Information and Event Management (SIEM), endpoint monitoring, the collection of logs and additional monitoring such as File Integrity Monitoring (FIM).</p>

<p>Overall, the project consisted of installing and deploying Wazuh through Docker onto a virtual machine hosted by Virtualbox, the virtual machine ran on Ubuntu Server version 24.04 LTS. After troubleshooting connectivity issues and a deployment onto a virtual machine without enough storage, I was able to simulate a small scale security monitoring environment, similar to what might be found within a SOC.</p>

<h2>Objectives:</h2>

<ul>

<li>Deploy a functional Wazuh SIEM environment</li>
<li>Configure a Wazuh Manager, Indexer and Dashboard</li>
<li>Deploy a Wazuh agent onto an Ubuntu server as an endpoint</li>
<li>Establish communication between the endpoint and Wazuh Manager</li>
<li>Monitor endpoint security events</li>
<li>Configure and test FIM</li>
<li>Understand the flow of information from endpoint to the SIEM</li>

</ul>

<h2>Environment</h2>

<p>
  The Wazuh Server was deployed using Docker Compose on an Ubuntu server, the environment included:
</p>

<ul>

<li>Wazuh Manager to process and analyse security events</li>
<li>Wazuh Indexer to store and index security data</li>
<li>Wazuh Dashboard to provide a web-based interface to analyse events</li>
<li>Docker / Docker Compose which was used to deploy and manage the components above</li>

</ul>

<p>
  Using the Wazuh Dashboard, it provided an interface that was used to monitor the environment from the server.
</p>

<h2>Wazuh Agents</h2>

<p>
  Utilizing Wazuh, I created an agent called Wazuh_Agent, which then was ran on the endpoint hosted by the Ubuntu server. This agent was used to monitor system activity, collect security data and securely forward the data gathered to the Wazuh Indexer for threat detection and analysis.
</p>

<p>
  The image below shows Wazuh_Manager active and functioning correctly.
</p>

<p>
  <img src="{{ "/assets/homelab/images/wazuhmanager/agent.png" | relative_url }}" alt="Wazuh Dashboard">
</p>

<h2>File Integrity Monitoring</h2>

<p>
  Through the use of Wazuh, the server was able to monitor specific files and directories for changes through the use of the agent. This can be used to identify suspicious activity within the environment, such as unauthorised modifications to system files.
</p>

<p>
  Below I used the agent created within the Wazuh Dashboard to analyze the actions carried out to create, edit then delete a file called wazuh-fim-test.txt. This was done to test the FIM.
</p>

<p>
  <img src="{{ "/assets/homelab/images/wazuhmanager/events.png" | relative_url }}" alt="Wazuh FIM Showcase">
</p>

<h2>Vulnerability Monitoring</h2>

<p>
  As well as being able to carry out FIM operations, the dashboard allowed me to view the individual vulnerabilities within the environment, where they were then categorised into different threat levels and then allowed for further analysis and planning how to help secure the server from said vulnerabilities.
</p>

<p>
  <img src="{{ "/assets/homelab/images/wazuhmanager/vulnerabilities.png" | relative_url }}" alt="Wazuh Vulnerability Showcase">
</p>

<p>
  Alongside this, Wazuh Dashboard also allowed me to inspect an inventory that contained all of the vulnerabilities, where I could freely use filters to track any specific event.
</p>

<p>
  <img src="{{ "/assets/homelab/images/wazuhmanager/inventory.png" | relative_url }}" alt="Wazuh Inventory Showcase">
</p>

<h2>Skills Demonstrated</h2>

<ul>

<li>SIEM Deployment</li>
<li>Wazuh Management</li>
<li>Docker &amp; Docker Compose</li>
<li>Troubleshooting</li>
<li>Security Event Monitoring</li>
<li>Analysis of logs and information forwarded to Wazuh</li>
<li>Service Management</li>
<li>Security telemetry pipelines</li>
<li>Incident investigation fundamentals</li>
<li>Configuration management</li>

</ul>

<h2>Conclusion</h2>

<p>
  This project gave me proper practical experience regarding how a real security monitoring environment functions, how to build it and how to troubleshoot it.
</p>

<p>
  Rather than simply installing Wazuh on an existing server, I had to create the endpoint, that being the Ubuntu server virtual machine, I established manager communication, investigated logs regarding FIM while validating it as a whole as well as followed security events through the monitoring pipeline.
</p>

<p>
  In conclusion, the project gave me a clearer understanding of many things regarding SIEMs, alongside how in the future I may present this information to a security analyst.
</p>
