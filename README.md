# GDPR-NIS2-Healthcare-SecOps-Lab

## 📌 Project Overview
This project demonstrates the end-to-end design, implementation, and security monitoring of a healthcare-grade IT infrastructure. The environment is specifically built to meet the rigorous standards of **GDPR** and the **NIS2 Directive**, focusing on data integrity, high availability, and proactive incident response.

The project simulates a Small-to-Medium Enterprise (SME) healthcare provider managing sensitive Electronic Health Records (EHR).

## 🏗️ Architecture
The infrastructure is built on a virtualized environment featuring:
* **Network Security:** pfSense Firewall with segmented VLANs (Management, EHR, DB, and VPN).
* **Monitoring & IDS:** Wazuh SIEM/HIDS and Suricata IDS for real-time threat detection.
* **Vulnerability Management:** Greenbone (OpenVAS) for continuous security auditing.
* **Incident Response:** IRIS-DFIR for professional case management and forensic documentation.



## 🛡️ Key Security Features
* **Data Protection by Design:** Implemented encryption-at-rest and strict Access Control Lists (ACLs).
* **Forensic Capability:** Developed workflows for disk imaging (`dd`) and volatile memory capture (`gcore`).
* **Compliance Mapping:** Every technical control is mapped to specific GDPR Articles and NIS2 requirements.

## ☣️ Simulated Scenarios & Response
The repository documents the detection and remediation of:
1. **Ransomware Attack:** Unauthorized encryption of the EHR server detected by Wazuh FIM.
2. **Data Exfiltration:** Large outbound data transfers from the Database segment identified via Suricata.
3. **Unauthorized Access:** Forensic investigation of a compromised VPN peer.

## 🛠️ Tools Used
* **Hypervisor:** VirtualBox / VMware
* **OS:** Kali Linux, Ubuntu Server, Metasploitable3
* **SIEM:** Wazuh
* **Firewall:** pfSense
* **Vulnerability Scanner:** OpenVAS / Greenbone Community Edition
* **Case Management:** IRIS-DFIR

## 📄 How to Read the Report
The full technical thesis, including configuration steps, forensic artifacts, and compliance audits, is available in the file:
👉 **[Design_and_Implementation_Healthcare_SME.pdf](./Design_and_Implementation_of_a_Secureand_Compliant_iT_Infrastructure_for_a_Healthcare_SME_under_GDPR_and_NIS2.pdf)**

---
*Created by Uthman Oluwadamilare Ismail - 2026*