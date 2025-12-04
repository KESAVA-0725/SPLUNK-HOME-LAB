# SPLUNK-HOME-LAB
This repository covers Installing Splunk, Splunk Apps, Data Ingestion and Parsing, Search Processing Language (SPL), and Dashboards and Log Analysis, providing all essential learning and practice materials for mastering Splunk fundamentals.

# Installing Splunk :

1. Open the official Splunk website (Splunk Enterprise page).

![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/images/download%20p2.png?raw=true)

2. Download Splunk Enterprise (Free trial: up to 500 MB/day for 60 days).

3. Choose the installer that matches your OS (Windows / Linux / macOS).

4. Run the installer and follow on-screen prompts.

5. During setup, create a local admin username and password when prompted.

6. Finish installation and start Splunk.

7. Access Splunk Web at http://localhost:8000
 (or http://<your-ip>:8000) and log in with the credentials you created.

# Splunk Apps
1. Identify the App/Add-on needed (e.g., Technology Add-on, CIM, Security Essentials).


# Data Ingestion and Parsing :

1. dentify your data sources (log files, CSV, JSON, syslog, Windows event logs, etc.).

![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/images/parsing.png?raw=true)

2. Choose an ingestion method: file monitor, HTTP Event Collector, syslog, universal forwarder, or scripted input.

3. Configure input in Splunk (Settings → Data Inputs) with correct source type and path/endpoint.

4. Ensure timestamps are recognized and timezone is correct.

5. Let Splunk parse events and assign default fields (source, sourcetype, host).

6. If needed, create or edit props.conf / transforms.conf to adjust parsing, line breaking, or field extractions.

7. Test with sample events and verify indexed fields in Search.

## Field Extraction in Splunk :

1. Splunk automatically extracts basic fields (like host, source, sourcetype, timestamp) using the file’s metadata.

2. When ingesting log data, Splunk also identifies common key-value pairs and auto-extracts them as searchable fields.

3. If the default extracted fields are not enough, we can manually create custom field extractions to parse additional information from the logs.

![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/images/Screenshot%202025-11-27%20181901.png?raw=true)

![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/images/Screenshot%202025-11-27%20182202.png?raw=true)

4. Using the Field Extractor (FX) or Regular Expressions (regex), we can highlight sample log entries and define new fields based on patterns in the data.

![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/images/Screenshot%202025-11-27%20182320.png?raw=true)

![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/images/Screenshot%202025-11-27%20182347.png?raw=true)

![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/images/Screenshot%202025-11-27%20182426.png?raw=true)

5. These custom fields make the logs easier to analyze, allowing Splunk to break unstructured text into meaningful attributes like usernames, IP addresses, URLs, actions, status codes, etc.

# Basic SPL Commands :

* search – Finds events in the index based on keywords, fields, or conditions.

* stats – Generates statistical summaries like count, sum, avg, max, etc.

* timechart – Creates time-based charts by grouping results over time.

* top – Shows the most frequently occurring values of a field.

* chart – Produces custom charts by grouping data into rows and columns.

* eval – Creates new calculated fields or modifies existing ones.

* rex – Extracts fields from raw events using regular expressions.

* spath – Extracts fields from JSON data structures.

* where – Filters results based on logical or comparison conditions.

* sort – Sorts events or statistical results in ascending/descending order.

* dedup – Removes duplicate events based on specified fields.

* Example : index=web sourcetype=access_combined | stats count by status

# Dashboards and Log Analysis 

1. First, decide what you want to monitor or investigate in your dashboard.

![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/images/dashboard%20p1.png?raw=true)

2. Write SPL queries that fetch the exact data or metrics you need.

3. Create dashboard panels like charts, tables, or single-value displays using those SPL queries.

 ![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/images/dashboard%20p2.png?raw=true)

4. Add interactive options such as a time picker or dropdown filters so users can easily adjust the dashboard view.

5. Under the Dashboards section, you can find and open all the dashboards you have created or saved.

 ![image](https://github.com/KESAVA-0725/SPLUNK-HOME-LAB/blob/main/images/dashboard%20p3.png?raw=true)
