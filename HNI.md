---
layout: default
---

![HNI Logo](/images/hni.png)

# HNI Corporation

---

### 🏢 Internship Overview

**Position:** Cybersecurity Intern  
**Location:** Muscatine, Iowa  
**Duration:** [May 2025 – August 2025]

---

### 📋 Duties

  * Filtered through the TRAP (Threat Response Auto Pull) inbox to manually review emails that that pose a phishing threat.
  * Also filtered through the DLP (Data Loss Prevention) inbox to ensure that no credit card or SSN numbers were sent in an email.
  * Participated in daily talks within the cybersecurity team to give updates and assess progress.
  * Participated in remediation simulations i.e. what would happen if the network became down.
  * Wiped and decommissioned old CISCO-ASA 5512-X firewalls.

---

### 🚀 Project

* Trusted Indicator Puller
**Objective:** The main project I worked on dealt with gathering trusted IP/CIDR addresses and automatically pushing them to all company firewalls.

* **Data Collection (Python):**
    * The first step was to make HTTP requests to different URLs hosting trusted CIDR ranges.
    * This was implemented completely in Python and designed to run efficiently from VS Code.
* **Integration (Cortex XSIAM):**
    * Created a feed integration within Cortex XSIAM to take the list of trusted IP addresses and publish them onto an **External Dynamic List (EDL)**.
    * This EDL was hosted on a URL that the firewalls were able to reference dynamically.
* **Change Detection:**
    * Developed a function to compare the old list of IP addresses against the new incoming list.
    * This provided visibility into which IP addresses were added or removed during each update cycle.
* **Firewall Configuration:**
    * Configured the firewalls by inputting the External Dynamic List URL into the firewall interface.
* **Outcome:** 
    * Once configured, the components worked together to automatically keep the firewall open for trusted IP addresses without manual intervention.

### 🧠 Skills Learned

**Technical Skills:**
* Cortex XSIAM
* Proofpoint TRAP and DLP
* Microsoft Teams and Outlook
* Python Scripting (Requests, Data Parsing)
* PuTTY / Cisco ASA Interface

**Soft Skills:**
* Technical communication within a team environment
* Time management and prioritization of tasks
* Professional communication (Coffee Talks, Seminars, Executive Talks)
* Problem-solving and critical thinking

---

### 📈 Evaluations

* Completed mid-term and final check-ins where my manager stated I met or exceeded expectations.
* Participated in performance reviews with HR representatives.
* **Outcome:** Was successfully offered a return offer.

---

### 🎤 Presentations

* Delivered a final presentation to the entire Information and Digital Technologies department.
* Shared the technical depth of the "Trusted Indicator Puller" project and explained its long-term benefits for future employees.
* Highlighted daily operational tasks and specific challenges overcome during the internship.
* Emphasized the impact of my work and received positive feedback from executives and senior employees.

---

[<<Back](./)
