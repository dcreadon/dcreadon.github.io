---
layout: default
---

# Secure Wireless Aircraft Data Load

![System Design](./SWADLArchitecture.png)
This is a high-level network architecture schematic of our design separating the Aircraft Information Service Domain (AISD) and Passenger Information and Entertainment Services Domain (PIESD).



## ✈️ Project Overview
**Client/Context:** Collins Aerospace (Prototype), Daniel Riechers  
**Focus:** Wireless Security, Wireless data Transfer, Embedded Systems (Raspberry Pi Device)  
**Role:** Security and Documentation Lead

This project addresses the potential for wireless data transfer in avionics. We designed and prototyped a Secure Wireless Data Loading system to replace traditional wired communication/loading. The goal was to demonstrate operational transfer of large payloads like In-Flight Entertainment (IFE) media and critical software updates between two devices on the aircraft.


## 🛠 Technology Stack

| Category | Technologies Used |
| :--- | :--- |
| **Hardware** | Raspberry Pi 5 (x2), Cisco 140ac WAP, Ubuntu Desktop |
| **Protocols** | EAP-TLS, 802.1x |
| **Security** | RADIUS (FreeRADIUS), X.509 Certificates, Device Authentication |
| **Compliance** | ARINC 615A, ARINC 665, ARINC 645 |

## 🏗 Architecture & Design

To mirror the constraints of an aircraft environment, we developed a design that is separated into two distinct domains: the AISD (Aircraft Information Service Domain) and PIESD (Passenger Information and Entertainment Services Domain).

### Hardware Implementation
* **Dataloader (Raspberry Pi 5):** Simulated using a Raspberry Pi. Acts as the source of critical updates.
* **Target System (Raspberry Pi 5):** Simulated using a Raspberry Pi. Represents the IFE (In-Flight Entertainment) system receiving the data.
* **Network Core (Access Point):** A Cisco 140ac Wireless Access Point serves as the bridge between domains.
* **Authentication Authority (RADIUS Server):** A physical Ubuntu Desktop hosting a RADIUS server handles certificate validation.

### Main Security Mechanism: EAP-TLS
As per our client, EAP-TLS (Extensible Authentication Protocol – Transport Layer Security) is the primary authentication method for devices.
* **Mutual Authentication:** Both the Raspberry Pi's must verify each other's identity through the access point and RADIUS server before a connection is established.
* **Isolated Network:** This configuration ensures an isolated environment for the devices to securely communicate on.

## 📜 Standards & Compliance
The system was designed around wirless avionic standards that are currently in place:

* **ARINC 615A:** Defined the transmission protocol for data loading over Ethernet/IP networks. 
* **ARINC 665:** Standardized the structure and file formats of Loadable Software Parts (LSP) to ensure correct installation of devices.
* **ARINC 645:** Handled data integrity and authentication via digital signatures and Cyclic Redundancy Checks (CRC) to prevent the loading of malicious software.

## 🧠 Skills & Knowledge Gained
Throughout the development of the project thus far, I have gained technical skill in three key areas:

* **Network Security:** Learned how to configure and deploy a freeRADIUS server from scratch using an Ubuntu Desktop. From this, I learned how to have the server create and manage certificates to make device authentication quick and secure.
* **Raspberry Pi Devices:** Developed skills on how to configure and use Raspberry Pi's. I also learned how to SSH into a Raspberry Pi. From there, I learned how to create an RDP session so the Pi desktop can be seen. Lastly, I learned how to conenct Raspberry Pi devices to a network so secure communication can occur. 
* **Linux Systems:** Configured and managed multiple Linux-based devices (Raspberry Pi's and Ubuntu Desktop). Configuration on these devices taught essential commands that should be known when creating a linux based system from scratch.

## Big Picture Contribution
This project serves as a possible alternative in avionic data transfer. By showing that secure wireless data loading is feasible, our prototype hopes to demonstrate that airlines can significantly reduce aircraft weight (by removing cabling and wired devices) and improve ground operation turnaround times, all while maintaining the strict safety and security standards required by the aviation industry.

**Website:** If you would like further detail on the project, refer to our team website located here: [SDMay26-36 Website](https://sdmay26-36.sd.ece.iastate.edu/).

[<<Back](./)