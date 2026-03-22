# azure-active-directory-soc-lab
Cloud-based Active Directory Setup lab on Microsoft Azure and User Management

---

## Project Overview

This project simulates a real-world enterprise identity and user access management infrastructure using **Microsoft Azure**. It demonstrates the deployment, configuration, and administration of a cloud-based **Active Directory (AD)** environment.

The lab focuses on:

- Provisioning domain controllers and domain-joined client VMs
- Configuring **AD DS**, DNS, and domain policies
- Creating organizational units and user accounts
- Managing user access and group memberships
- Observing Windows Security Event Logs relevant to SOC operations

Although this project does not include direct log analysis, it establishes a **strong foundation for SOC monitoring**, as AD events generate security logs that are critical for threat detection.

---

## Project Architecture

**Environment:**

- **Resource Group:** ActiveD-LAB
- **Virtual Network:** ActiveD-VNet
- **Domain Controller VM:** Domain-Controller01 (Windows Server 2022)
- **Client VM:** Client01 (Windows Server 2022, domain-joined)

**Core Components:**

- Active Directory Domain Services (AD DS)
- Domain controller and client workstation
- Organizational Units (OU) and user accounts
- Windows Security Event Logs for authentication and account activity

---

## Key Features Demonstrated

1. **Domain Controller Setup**
   - Promote VM to domain controller
   - Configure DNS and AD DS
   - Create administrative accounts

2. **Client Integration**
   - Join client VM to domain
   - Configure DNS to point to domain controller
   - Verify domain authentication

3. **User and OU Management**
   - Create Organizational Units and Users (e.g., Alice, Bob, Charlie)
   - Reset passwords and assign group memberships
   - Simulate enterprise identity lifecycle

4. **Security Event Log Monitoring**
   - Identify key Active Directory Event IDs for SOC relevance:
     - **4624:** Successful logon
     - **4625:** Failed logon
     - **4720:** User account creation
     - **4732:** User added to security group
   - Prepare for SOC monitoring and SIEM integration

---
## 📌 Conclusion
This project provides a foundational understanding of Active Directory in a cloud environment and demonstrates how identity-based activities generate critical security logs.

It highlights the role of SOC analysts in monitoring authentication events, detecting suspicious behavior, and responding to potential threats within enterprise environments.

---

## 👤 Author
Abubakar Yusuf  
SOC Analyst 
