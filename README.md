# Network-Traffic
A full digital forensics investigation performed on a captured PCAP file during a simulated cyberattack. The project includes host identification, FTP credential extraction, malicious file recovery, NTLM hash cracking, steganography analysis, and hidden message discovery using tools such as Wireshark, Steghide, John the Ripper, CrackStation.

# 🕵️‍♂️ Network Traffic Analysis – Digital Forensics Investigation  
**Author:** Adeseye Nelson Olaiyapo  
**Date:** 28/02/2026  
**Tools:** Wireshark, Steghide, John the Ripper, Hashcat, CrackStation, zsteg, binwalk, unrar  



## 📌 Project Overview  
This project documents a full digital forensics investigation performed on a captured network traffic file (PCAP) during a simulated cyberattack. The objective was to analyze the traffic, extract evidence, recover hidden data, and answer key investigative questions related to the attacker’s activities.

The investigation involved protocol analysis, file extraction, password cracking, and steganography techniques to uncover the attacker’s actions and hidden messages.



## 🎯 Objectives  
The analysis focused on identifying:

1. **Target machine IP address**  
2. **FTP username used by the attacker**  
3. **Executable file uploaded via FTP**  
4. **Administrator password (NTLM hash cracked)**  
5. **Hidden “secret” message embedded in website image files**



## 🛠️ Methodology  
### **Tools Used**
- **Wireshark** – Protocol analysis, stream reconstruction, object extraction  
- **Steghide / zsteg / binwalk** – Steganography and hidden data extraction  
- **John the Ripper / Hashcat / CrackStation** – Password and hash cracking  
- **Exiftool, unrar** – Metadata and archive extraction  

### **Workflow**
1. Identified active hosts and suspicious traffic  
2. Analyzed FTP/HTTP sessions  
3. Extracted transferred files and web objects  
4. Performed steganography analysis on PNG images  
5. Cracked NTLM hashes to recover credentials  
6. Correlated all findings to answer investigation questions  



## 🔍 Key Findings  
### **1. Target Machine IP**  
**192.168.158.131**  
(Identified via conversation analysis and TCP handshake inspection)

### **2. FTP Username**  
**anonymous**  
(Recovered from FTP control stream)

### **3. Uploaded Executable**  
**PwDump7.exe**  
(Extracted via FTP STOR command and object export)

### **4. Administrator Password**  
**123456**  
(Cracked from NTLM hash using John the Ripper, Hashcat, and CrackStation)

### **5. Hidden “Secret” Message**  
**Hidden_st3g**  
(Extracted using zsteg, binwalk, and RAR password cracking)



## 📂 Project Structure
/Network-Traffic-Analysis
│── PCAP Analysis
│── FTP & HTTP Evidence
│── Extracted Files
│── Hash Cracking Results
│── Steganography Findings
│── Screenshots & Documentation
│── Report.pdf / Report.docx


## 🔐 Recommendations  
- Enforce encrypted protocols (SFTP/FTPS, HTTPS)  
- Monitor and alert on unusual FTP uploads  
- Perform regular file integrity checks  
- Harden authentication and password policies  



## 📄 Conclusion  
This investigation successfully uncovered the attacker’s activities, extracted hidden data, cracked credentials, and reconstructed the attack path. The project demonstrates practical skills in network forensics, steganography, password cracking, and evidence correlation.


## ⭐ If you find this project useful, consider giving the repository a star!
