# SOC-ANALYSIS-LAB
Simple Home-Lab (Active Directory) to Practice SOC Analysis

👉 Download Virtualbox: https://www.virtualbox.org/wiki/Downloads
👉 Download Windows 10
👉 Install Windows Server 2019 [180 days Trial] https://info.microsoft.com/ww-landing-windows-server-2019.html?lcid=en-IN
👉 Set up Domain Controller for Active Directory https://www.ibm.com/docs/en/storage-scale-bda?topic=support-install-configure-active-directory

🛡️ Download any one of them (ELK, QRadar)SIEM
🔰 Elastic ELK SIEM
🔰 ELK's architecture:
✔ Elastic's ELK is an open-source stack for managing and analyzing large volumes of data.  The ELK stack consists of three applications (Elasticsearch, Logstash, and Kibana ).

✔ Elasticsearch is a NoSQL database based on the Lucene search engine and built with RESTful APIs. It is essentially the index, store, and query application of the ELK stack.

✔ Logstash is the tool responsible for the collection, transformation, and transport of log file records.

✔ Kibana is the tool used for visualizing the Elasticsearch documents.

✔ Beats is an additional download that should be installed in every remote location for its logs to be shipped to the Logstash component.
https://www.elastic.co/guide/en/siem/guide/current/siem-overview.html
____________________________________________
🔰 Process of how data flows from Beats to Kibana in the Elastic ELK stack:
1. Data collection: Beats collects data from different sources, such as logs, metrics, or network packets, and sends them to Logstash or Elasticsearch directly.

2. Data processing: If the data is sent to Logstash, it goes through a series of filters where it can be parsed, Transformed, and Enriched before being sent to Elasticsearch. Logstash can also handle data enrichment, such as adding geo-location data or user agent information.

3. Data indexing: Elasticsearch then indexes the data, making it searchable and available for analysis.

4. Data visualization: Kibana is used to visualize and analyze the data stored in Elasticsearch. Users can create custom dashboards, visualizations, and reports to gain insights into the data. Kibana also provides a user-friendly interface for exploring the data and filtering results, and using lucene query search to
____________________________________________

🔰 Download:
- Elasticsearch - https://www.elastic.co/downloads/elasticsearch
- Kibana - https://www.elastic.co/downloads/kibana
- Elastic-agent - https://www.elastic.co/downloads/elastic-agent
- Beat - https://www.elastic.co/downloads/beats
- Logstash - https://www.elastic.co/downloads/logstash

🔰 Installing the Elastic Stack - https://www.elastic.co/guide/en/elastic-stack/current/installing-elastic-stack.html

🔰 Lucene query syntax is available to Kibana users who opt out of the Kibana Query Language. - https://www.elastic.co/guide/en/elasticsearch/reference/6.7/query-dsl-query-string-query.html#query-dsl-query-string-query

👉 Elastic Free Courses - https://www.elastic.co/training/free

🛡️ QRadar
Download > https://www.ibm.com/community/qradar/ce/
install > https://www.youtube.com/watch?v=DCd5f4VFDdk

__
✔️ All material you need:- 
. WinCollect Agent: https://bit.ly/3xhioeb
. 730_QRadar_wincollectupdate-7.3.1-16.sfs: https://bit.ly/3xdPzPS
. WinSCP-5.21.3-Setup: https://bit.ly/3QsblpO
. CCNA Cyber Ops SECOPS: https://bit.ly/3L0W6Dj
. DSM Configuration Guide: https://ibm.co/3dhP9Bl
. Incident Handling and Response: https://bit.ly/3QPvDtJ
. What is SIEM: https://bit.ly/3dkIohW


✔️ If you encounter any of these issues below, I've collected the solutions.

__
. install WinCollect Agent another way:
https://www.youtube.com/watch?v=CI6g5brdSdw 
https://www.youtube.com/watch?v=ZgbHcp0IUI 

__
. send Linux logs to Qradar
https://www.youtube.com/watch?v=z3XezJnGtq0

___
. No Log Activity | Qradar CE 
https://www.youtube.com/watch?v=IwkEm772EZI

__
. No Log Activity | Qradar Code:
https://www.ibm.com/support/pages/node/6395080

__
. Logs source problem:
https://exchange.xforce.ibmcloud.com/hub/extension/8169c48dc992961acb8f963cdcf56faa

__
. Modify maximum Log size using Group Policy
https://www.youtube.com/watch?v=LeUx8EGFKXE

__
. Rule creation, use case creation Basic in Qradar SIEM
https://www.youtube.com/watch?v=M4-ESZgZZBk |
https://ibm.co/3DwndEq

✔️ Don't forget to generate an Authentication token from AS to write in WinCollect Agent when you install it 
____

✔️ where logs and events from Windows, Linux, DB,..,etc :
 . DSM Configuration Guide: https://ibm.co/3dhP9Bl
___

--> Does it work? Great! That is a mini SOC. Document it somewhere and link it to your resume.🙏

____

------> Additional steps: <------

- Increase log visibility (activate PowerShell logging, Scriptblock logging, install Sysmon, etc)

- Install extra tools to get more visibility e.g.: Bluespan, DeepBlueCLI, Suricata Zeek, RITA (all are on GitHub)

- Test your setting! Be a bad guy and try to catch yourself. (WinPwn, Atomic Red Team, Caldera -> again, check out GitHub)

- If needed improve your SIEM with matching alert rules and build Dashboards. (Ideas? Look at Sigma rules -> GitHub)

- Threat Intelligent Cyber Threats and Where to Find Them :
socprime.com
- Insert your IOCs, and get queries on the fly:
cti.uncoder.io

🎯 For more content - https://www.linkedin.com/in/praise-ordu-049a95109/
👉QRadar - Jose Bravo - https://www.youtube.com/watch?v=P90e4iEJ32s&
Credit goes to Mohammed Eissa  https://www.linkedin.com/in/mohessa511/
Check out my Free course on Introduction to Cybersecurity: https://cybersectechacademy.thinkific.com/
🔰 SOC SIEM Use Cases
🛡️ Below is a list of sample use cases. You can categorize it in multiple ways.
👉 Windows Use Cases
Server Shutdown/ Reboot
Removable media detected
Windows abnormal shutdown
Login attempts with the same account from different source desktops
Detection of Server shutdown-reboot after office hours
Administrative Group Membership Changed
Unauthorized Default Account Logins
Interactive use of service account
Remote access login – success & failure
Windows Service Stop-Restart
ACL Set on Admin Group members
Windows Account Enabled Disabled
Multiple Windows Account Locked out
Multiple Windows Logins by Same User
Brute force attempt from the same source
Logins outside normal business hours
Logins to multiple users accounts from the same source.
Brute force attempt from the same source with a successful login.
Windows Account Created Deleted
Windows Hardware Failure
Failed Login to Multiple Destinations from Same Source
Administrative Accounts- Multiple Login failure
Detection of user account added/removed in admin group
Detection of system time changes (Boot time)
Detection of use of default product vendor accounts
User Deleted Within 24hrs of Being Created
Critical service stopped on Windows Servers
Windows Security Log is full
Multiple Password Changes in a Short time period
Windows group type was changed.
Audit Policy change
Audit Log cleared
Windows Security Log is full
Detection of user account added
Logon Failure-A logon attempt was made using an expired account
High number of users created/ removed within a short period of time
Outbound Traffic observed from Severs to Internet.
Failed Logins/Attempt with Disabled/Ex-Employee/Expired Accounts
Windows File-Folder Delete
Windows-File Folder Permission Changes
High number of users were created/removed within a short period of time

> Document and show your skills on your resume.

Why?

If you take a cert like Sec+ can you do your job?
-Off Course 
