# Intune + Windows 11 + Hyper-V Lab

## Overview
This lab demonstrates the end-to-end deployment, enrollment, and management of a Windows 11 virtual machine using **Microsoft Intune** and **Microsoft Entra ID (Azure AD)**.

The project was built to showcase real-world endpoint management skills, including device enrollment, license troubleshooting, and application deployment in an enterprise-style environment.

---

## Lab Objectives
- Create a Windows 11 virtual machine using Hyper-V
- Enable TPM and Secure Boot for Windows 11 compatibility
- Enroll the device into Microsoft Entra ID
- Enable Microsoft Intune (MDM) management
- Troubleshoot Intune enrollment errors
- Deploy Microsoft Edge using Intune
- Verify policy and application deployment on the endpoint

---

## Technologies Used
- Windows 11 Enterprise (Evaluation)
- Hyper-V
- Microsoft Entra ID (Azure AD)
- Microsoft Intune
- Microsoft 365 Business Premium
- Microsoft Edge (Enterprise)

---

## Lab Architecture
- Host: Windows 10/11 with Hyper-V enabled
- Guest VM: Windows 11 (Generation 2)
- Identity: Microsoft Entra ID (Cloud-only)
- Device Management: Microsoft Intune (MDM)
- Application Deployment: Intune Windows app (Microsoft Edge)

---

## Implementation Summary

### 1. Windows 11 VM Deployment
- Created a Generation 2 Hyper-V virtual machine
- Enabled TPM and Secure Boot
- Installed Windows 11 successfully

### 2. Microsoft Entra ID & Intune Configuration
- Assigned Microsoft 365 Business Premium license
- Enabled MDM user scope = **All**
- Verified Intune tenant status
- Resolved enrollment error **0x80180018** by correcting license assignment

### 3. Device Enrollment
- Connected VM to **Work or School account**
- Successfully joined Microsoft Entra ID
- Device appeared in Intune portal
- Verified MDM connection on the VM

### 4. Application Deployment (Microsoft Edge)
- Added **Microsoft Edge for Windows 10 and later** via Intune
- Assigned application as **Required**
- Synced device from Intune
- Verified Edge presence and policy status using:
  - `edge://policy`

---

## Validation & Evidence
- Device visible in Microsoft Intune
- Device shows **Entra ID + MDM connected**
- Microsoft Edge assigned successfully
- Edge policies visible on the VM

---

## Skills Demonstrated
- Windows 11 virtualization with Hyper-V
- Microsoft Entra ID device join
- Microsoft Intune MDM configuration
- Troubleshooting Intune enrollment errors
- Application deployment via Intune
- Policy verification and validation
- Enterprise endpoint management fundamentals

---

## Screenshots & Evidence

> Screenshots are stored in this directory and referenced as evidence of successful deployment, enrollment, and policy application.

---

## Notes
This lab was created as part of my IT portfolio to demonstrate hands-on experience with modern endpoint management and cloud identity solutions.
