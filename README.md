# VirusTotal Malware Analysis Project

## 📌 Project Overview

This project demonstrates practical malware analysis using **VirusTotal** by analyzing multiple real-world samples through hash-based investigation. The objective is to understand malware detection, behavior indicators, false positives, and SOC-style verdicts without executing any malicious code.

The project was completed as part of a **cybersecurity internship task**, following safe and ethical analysis practices.

---

## 🎯 Objectives

* Perform hash-based malware analysis using VirusTotal
* Interpret antivirus detection results
* Analyze behavioral indicators and sandbox reports
* Differentiate between real malware and false positives
* Present findings in a SOC-analyst reporting format

---

## 🛠 Tools & Platform

* **VirusTotal** (Static & Dynamic Analysis)
* **MITRE ATT&CK Mapping**
* **Crowdsourced YARA & Sigma Rules**

---

## 📂 Sample Summary

| Sample   | File Type          | Classification                      | Detection Ratio |
| -------- | ------------------ | ----------------------------------- | --------------- |
| Sample 1 | Android APK        | Suspicious / Low-confidence Malware | 33/68           |
| Sample 2 | Test File (EICAR)  | Antivirus Test Malware              | 65/67           |
| Sample 3 | Windows Executable | Ransomware (WannaCry)               | 67/71           |
| Sample 4 | JavaScript File    | Benign / False Positive             | 0/59            |

---

## 🔍 Detailed Analysis

### 🧪 Sample 1 – Android Malware (Low Confidence)

* Partial antivirus detections
* Obfuscated code and SMS-sending behavior
* Limited behavioral indicators
* Classified as **suspicious**, not conclusively malicious

**Verdict:** Requires further monitoring

---

### 🧪 Sample 2 – EICAR Test File

* Known antivirus test string
* Detected by almost all vendors
* No real malicious functionality

**Verdict:** Test malware (safe, non-harmful)

---

### 🧪 Sample 3 – Ransomware (WannaCry)

* Strong signature-based detection
* Matches WannaCry YARA rules
* Extensive malicious behavior:

  * File encryption
  * Persistence mechanisms
  * Network communication
  * Anti-analysis techniques

**Verdict:** Confirmed ransomware threat

---

### 🧪 Sample 4 – False Positive Case

* Zero detections across all vendors
* No behavioral indicators
* Extremely small and inert file

**Verdict:** Benign / False Positive

---

## 🧠 MITRE ATT&CK Highlights

* Execution (T1059)
* Persistence (T1547)
* Defense Evasion (T1562)
* Command and Control (T1071)

*(Observed primarily in Sample 3)*

---

## ✅ Key Learnings

* High detection ≠ always real malware (EICAR case)
* Low detection ≠ always benign (Sample 1)
* Behavioral evidence is critical in malware confirmation
* False positives must be carefully validated to reduce SOC alert fatigue

---

## ⚠️ Ethical & Safety Notice

* No malware was downloaded or executed locally
* Analysis was conducted using **hashes only**
* Project follows ethical cybersecurity guidelines

---

## 📌 Conclusion

This project demonstrates real-world SOC analysis skills including threat validation, false positive handling, and professional reporting. It reflects industry-aligned practices expected from entry-level SOC and cybersecurity interns.

---

## 👤 Author

**Parijat Das**
Cybersecurity Enthusiast | SOC & Malware Analysis Learner

---

⭐ *If you find this project useful, consider giving it a star!*
