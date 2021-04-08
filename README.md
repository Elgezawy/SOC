# SOC

pcap is an application programming interface (API) for capturing network traffic. ... 
PCAP file creates a record of network data that you can view through Wireshark

(ZEEK LOGS)..
formerly Bro)[2] is a free and open-source software network analysis framework
Zeek sits on a “sensor,” a hardware, software, virtual,
 or cloud platform that quietly and unobtrusively observes network traffic. 
Zeek interprets what it sees and creates compact,
 high-fidelity transaction logs,
 file content, and fully customized output,
 suitable for manual review on disk or in a more analyst-friendly tool like a security and information event management (SIEM) system.

₩ The following Zeek log files are updated daily:
• known_hosts.log: Log file containing information for hosts that completed TCP 
handshakes.
• known_services.log: Log file containing a list of services running on hosts.
• known_certs.log: Log file containing a list of Secure Socket Layer (SSL) certificates.
• software.log: Log file containing information about Software being used on the 
network.

₩ Additionally, a list of detection-based log files is created during each session. The log files 
relevant to this lab are:
• notice.log (Zeek notices): When Zeek detects an anomaly, a corresponding notice 
will be raised in this file.
• intel.log (Intelligence data matches): When Zeek detects traffic flagged with 
known malicious indicators, a corresponding reference will be logged in this file.
• signatures.log (Signature matches): When Zeek detects traffic flagged with known 
malicious or faulty packet signatures, a corresponding reference will be logged in 
this file

₩ process pcap file with zeex:
zeek -r smallFlows.pcap

₩ list files generated with zeex: ls

...........................

( BRIM )
-you can open a pcap with Brim and it will transform the pcap into Zeek logs in the ZNG format

-Wireshark has one glaring flaw--it doesn't handle large capture files with much grace


















