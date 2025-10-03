---
layout: default
---

![HNI Logo](/images/hni.png)

# HNI Corporation

---

### Internship Overview

**Position:** Cybersecurity Intern  
**Location:** Muscatine, Iowa  
**Duration:** [May 2025 – August 2025]

---

### Duties

  - Filtered through the TRAP (Threat Response Auto Pull) inbox to manually review emails that that pose a phishing threat.
  - Also filtered through the DLP (Data Loss Preventio) inbox to ensure that no credit card or SSN numbers were sent in an email.
  - Participated in daily talks within the cybersecurity team to give updates and assess progress.
  - Participated in remediation simulations i.e. what would happen if the network became down.
  - Wiped and decommissioned old CISC-ASA 5512-X firewalls.

---

### Project

- Trusted Indicator Puller
  - The main project I worked on over the summer dealt with gathering trusted IPs and pushing them to the firewalls.
  - The first step of the project was to make HTTP requests to differnt URLs hosting trusted CIDR ranges.
  - This step was implemented completely in python and could run straight from vs code.
  - The second step of the project, was to make a feed integration within Cortex XSIAM.
  - This feed integration was able to take the list of these IP addresses and publish them onto an External Dynamic List.
  - This external dynamic list was hosted on a URL that the firewalls were able to reference.
  - The third step was to create a function that was able to check the old list of IP addresses against the new incoming list.
  - This allowed for visibility on seeing which IP addresses were removed or added from the list.
  - The final step, was to configure the firewalls.
  - To do this, I just had to input the external dynamic list URL into the firewall interface. 
  - Once the firewall was configured, each component began working together to keep the firewall open for trusted IP addresses.

### Skills Learned

**Technical Skills:**
  - Cortex XSIAM
  - ProofPoint TRAP and DLP
  - Microsoft Teams and Outlook
  - Python
  - PuTTy, specifically CISCO ASA Interface

**Soft Skills:**
  - Technical communication within a team environment
  - Time management and prioritization of tasks
  - Professional Communication within a workplace (Coffee Talks, Seminars, Executive Talks)
  - Problem-solving and critical thinking

---

### Evaluations
  - Had a mid-term and final check-in where my manager believed I met/exceeded expectations.
  - Had additional meetings with my HR representative about my performance and how I was doing.
  - Was offered a return job.

---

### Presentations

  - Delivered a final presentation to the entire Information and Digital Technologies department on my project and other tasks.
  - Shared the depth of my project and explained how it could be beneficial to the company for future employees.
  - Shared other tasks that I performed on a daily basis along with some other challenging ones I was assigned.
  - Emphasized how I was able to make an impact over the summer and a beneficial intern.
  - Had the opportunity of receiving feedback on my presentation from executives and other employees. 

---
