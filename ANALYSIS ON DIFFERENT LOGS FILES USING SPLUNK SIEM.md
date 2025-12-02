# Log Analysis of Different Log Types Using Splunk SIEM

In this project, I worked on analyzing different types of logs using Splunk SIEM. These logs help us understand what is happening in the network and find any unusual or suspicious activity. I analyzed DNS, DHCP, HTTP, and SMTP logs.
Below, I will attach the sample log files and explain each log type in simple words.

# 1. DNS Log Analysis

Attaching the Sample lof file for practice.

Obtain sample DNS log file in a suitable format (e.g., text files).

Ensure the log files contain relevant DNS events, including source IP, destination IP, domain name, query type, response code, etc.

Save the sample log files in a directory accessible by the Splunk instance.

# 2. DHCP Log Analysis

Obtain sample  in a suitable format.

Ensure the log files contain relevant DHCP events, including timestamps, IP address assignments, lease durations, client identifiers, etc.

Save the sample log files in a directory accessible by the Splunk instance.

# 3. HTTP Log Analysis

Obtain sample HTTP log files in a suitable format (e.g., text files).

Ensure the log files contain relevant HTTP events, including timestamps, request methods, URLs, response codes, user agents, etc.

Save the sample log files in a directory accessible by the Splunk instance.

# 4. SMTP Log Analysis

Obtain sample SMTP log file in a suitable format (e.g., text files).

Ensure the log files contain relevant SMTP events, including timestamps, sender and recipient addresses, email subjects, etc.

Save the sample log files in a directory accessible by the Splunk instance.


# Sample SPL queries used for analyzing the HTTP log data are given below

# 1. Search for HTTP Events :

Open Splunk interface and navigate to the search bar.

Enter the following search query to retrieve SMTP events

=>>>   Example : index=<your_smtp_index> sourcetype=<your_smtp_sourcetype>    <<<=

![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/Entering%20view.png?raw=true)


# 2. Analyze Web Traffic Patterns

1. ![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/sample%201.png?raw=true)

  ===========================================================================================

2. ![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/sample%202.png?raw=true)

  ===========================================================================================

3. ![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/sample%203.png?raw=true)

 ===========================================================================================

4. ![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/sample%204.png?raw=true)

   =========================================================================================

5.![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/sample%205.png?raw=true)

