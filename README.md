# Ransomware Behavior Analysis Using Cowrie Honeypot
This project focuses on ransomware behavior analysis using a Cowrie SSH honeypot deployed in a controlled virtual environment. A Kali Linux virtual machine was configured to host the Cowrie honeypot, while an Ubuntu virtual machine was used to simulate attacker activities. The honeypot was configured to listen for SSH connections on port 2222 and successfully captured login attempts, executed commands, session details, and attacker interactions. During the experiment, reconnaissance commands such as `uname -a`, `whoami`, and `pwd` were executed from the attacker machine to simulate the initial stages of a cyberattack. The generated logs were collected and analyzed to understand attacker behavior and system interaction patterns. Elasticsearch was installed and configured for log management and indexing, while Python scripts were developed to calculate interaction statistics and generate attack timelines. Matplotlib was used to visualize attacker behavior through graphical representations. A total of 19 interactions were successfully captured and analyzed. The project demonstrates how honeypots can be used as an effective security monitoring solution to detect, record, and analyze suspicious activities before a potential ransomware attack progresses further.

## Objectives

* Deploy a Cowrie SSH honeypot
* Capture attacker interactions
* Analyze collected logs
* Visualize attack behavior
* Explore geolocation and threat monitoring concepts

## Technologies Used

* Kali Linux
* Ubuntu Linux
* Cowrie Honeypot
* Python
* Elasticsearch
* Matplotlib
* VirtualBox
* SSH

## Project Architecture

Attacker Machine (Ubuntu)
↓
SSH Connection
↓
Cowrie Honeypot (Kali)
↓
Cowrie Logs
↓
Elasticsearch
↓
Python Analysis
↓
Matplotlib Visualization

## Results

* Total interactions recorded: 19
* Successful SSH login captured
* Reconnaissance commands detected:

  * uname -a
  * whoami
  * hostname
  * pwd
  * find . -type f
  * cat /etc/passwd
  * etc
* Elasticsearch deployed and verified
* Python log analysis completed
* Visualization generated using Matplotlib


## Future Improvements

* Kibana dashboard integration
* GeoIP enrichment
* Real-time alerting
* Machine learning-based anomaly detection

## Author
Mekala Shanvithkar
