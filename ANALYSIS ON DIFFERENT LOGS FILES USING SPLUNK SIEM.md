# Log Analysis of Different Log Types Using Splunk SIEM

In this project, I worked on analyzing different types of logs using Splunk SIEM. These logs help us understand what is happening in the network and find any unusual or suspicious activity. I analyzed DNS, DHCP, HTTP, and SMTP logs.
Below, I will attach the sample log files and explain each log type in simple words.

# 1. DNS Log Analysis

(Sample DNS log file will be added here)
DNS logs show which websites or domains were looked up by users. They help us find suspicious domain activity.

# 2. DHCP Log Analysis

(Sample DHCP log file will be added here)
DHCP logs show which devices joined the network and what IP address they received. Useful for tracking unknown devices.

# 3. HTTP Log Analysis

(Sample HTTP log file will be added here)
HTTP logs show details about website visits, requests, and responses. They help identify errors and suspicious web activity.

# 4. SMTP Log Analysis

(Sample SMTP log file will be added here)
SMTP logs show email sending activity. They help detect spam, phishing, or any unusual email behavior.

# Sample SPL queries used for analyzing the HTTP log data are given below

# 1. Search for HTTP Events :

Open Splunk interface and navigate to the search bar.

Enter the following search query to retrieve SMTP events

=>>>   Example : index=<your_smtp_index> sourcetype=<your_smtp_sourcetype>    <<<=


# 2. Analyze Web Traffic Patterns

![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/sample%201.png?raw=true)
![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/sample%202.png?raw=true)
![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/sample%203.png?raw=true)
![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/sample%204.png?raw=true)
![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/sample%205.png?raw=true)

