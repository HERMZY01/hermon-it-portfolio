
# Intune + Windows 11 + Hyper-V Lab

## Overview
This lab demonstrates how to deploy, enroll, and manage a Windows 11 virtual machine using Microsoft Intune and Microsoft Entra ID (Azure AD).

The goal of this project is to show practical, hands-on experience with:
- Windows 11 device enrollment
- Microsoft Intune configuration
- Microsoft Edge deployment via Intune
- Hyper-V virtualization

This lab was built as part of my IT portfolio to demonstrate real-world endpoint management skills.


---

## Lab Objectives
- Create a Windows 11 virtual machine using Hyper-V
- Enroll the VM into Microsoft Entra ID
- Enable Intune MDM management
- Resolve common Intune enrollment errors (0x80180018)
- Deploy Microsoft Edge using Intune
- Verify policy and app deployment on the device

---

## Technologies Used
- Windows 11 Enterprise (Evaluation)
- Hyper-V (Windows 10/11 host)
- Microsoft Intune
- Microsoft Entra ID (Azure AD)
- Microsoft Edge (Windows catalog app)

---

## Lab Architecture
Host PC  
→ Hyper-V  
→ Windows 11 VM  
→ Microsoft Entra ID  
→ Microsoft Intune  

---

## Step-by-Step Summary

### 1. Hyper-V Setup
- Enabled Hyper-V on host machine
- Created Generation 2 Windows 11 VM
- Enabled TPM and Secure Boot
- Installed Windows 11 successfully

### 2. Microsoft Entra ID & Intune Configuration
- Assigned Microsoft 365 Business Premium license
- Enabled MDM user scope = **All**
- Verified Intune tenant status
- Resolved enrollment error **0x80180018** by correcting license assignment

### 3. Device Enrollment
- Connected VM to Work or School account
- Successfully joined Entra ID
- Device appeared in Intune portal
- Verified MDM connection on the VM

### 4. Application Deployment (Microsoft Edge)
- Added **Microsoft Edge for Windows 10 and later**
- Assigned app as **Required**
- Synced device
- Verified Edge presence and policy status via:
  - `edge://policy`

---

## Validation & Evidence
- Device visible in Intune portal
- Microsoft Edge app assigned successfully
- Device shows as Entra ID + MDM connected
- Edge policies visible on VM

---

## Skills Demonstrated
- Endpoint Management (Intune)
- Azure AD / Entra ID
- Windows 11 administration
- Virtualization (Hyper-V)
- Troubleshooting enrollment & licensing issues
- App deployment and validation

---

## Why This Matters
This lab mirrors real enterprise scenarios:
- Corporate device onboarding
- License misconfiguration troubleshooting
- Cloud-managed Windows environments

It demonstrates job-ready skills for roles such as:
- IT Support Engineer
- Microsoft 365 Engineer
- Endpoint Administrator
- Junior Cloud Engineer

---

## Author
**Hermon Browne**  
IT Support | Microsoft 365 | Intune | Windows  

