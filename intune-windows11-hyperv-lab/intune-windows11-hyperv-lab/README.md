
# Intune + Windows 11 + Hyper-V Lab

## Overview
This lab demonstrates how to deploy a Windows 11 VM in Hyper-V, join it to Microsoft Entra ID, enroll it into Microsoft Intune (MDM), and deploy Microsoft Edge via Intune.

## Why this matters (real-world relevance)
Organizations use Intune + Entra ID to control devices, deploy apps, enforce policies, and validate compliance. This lab mirrors a typical onboarding + management workflow used in modern IT teams.

## Lab Objectives
- Build a Windows 11 VM using Hyper-V (TPM + Secure Boot)
- Join device to Microsoft Entra ID (work/school)
- Enable MDM enrollment into Microsoft Intune
- Fix common enrollment error `0x80180018`
- Deploy Microsoft Edge via Intune
- Validate deployment and policy status on the device

## Technologies Used
- Windows 11 Enterprise Evaluation (VM)
- Hyper-V (Gen 2 VM)
- Microsoft Entra ID (Azure AD)
- Microsoft Intune (Endpoint Manager)
- Microsoft 365 Business Premium (license)



**Hyper-V VM** → **Entra ID Join** → **Intune MDM Enrollment** → **App Deployment (Edge)** → **Validation (edge://policy + Intune status)**

---

# Step-by-step Implementation

## 1. Hyper-V VM Build (Windows 11 Requirements)
**Key actions**
- Created Generation 2 VM
- Enabled Secure Boot
- Enabled TPM 2.0 (virtual TPM)

**Evidence**
- ![Windows 11 setup TPM requirement

---

## 2. Entra ID + Intune Tenant Configuration
**Key actions**
- Verified Intune tenant status
- Confirmed MDM user scope = **All**
- Confirmed Intune license assignment for enrollment user

  

---

## 3. Device Enrollment (Windows 11 VM → Intune)
**Key actions**
- Connected the VM to Work or School account (Entra ID join)
- Enrolled into Intune (MDM connected)

**Troubleshooting**
- Hit enrollment issue: `0x80180018`
- Fixed by correcting license assignment to the enrolling user
- Enrollment succeeded after license + MDM user scope were correct

-

---

## 4. Application Deployment (Microsoft Edge)
**Key actions**
- Added **Microsoft Edge for Windows 10 and later** in Intune Apps
- Assigned deployment as **Required** to the device/user group
- Forced sync from device



---

# Validation & Evidence
✅ Device appears in Intune  
✅ Device shows Entra ID + MDM connected  
✅ Microsoft Edge deployment assigned successfully  
✅ Policy and management verified using:
- `edge://policy`

---

# Troubleshooting Notes (What I learned)
## Error: 0x80180018 (Enrollment failed / Server error)
**Likely causes**
- Missing Intune license for the enrolling user
- MDM user scope not enabled
- Enrollment restrictions blocking Windows

**Fix used**
- Assigned valid license to the enrolling user
- Confirmed **MDM user scope = All**
- Retried enrollment → succeeded

---

## Next Improvements
- Deploy a Win32 app (7-Zip or Notepad++)
- Add a Compliance Policy (BitLocker/Password/Firewall)
- Add a Configuration Profile (Edge settings, OneDrive KFM, etc.)
- Add Conditional Access policy (require compliant device)

- ### Troubleshooting workflow used
1. Confirm user licensing (M365/Intune)
2. Confirm MDM user scope enabled
3. Check device join state (Entra ID joined)
4. Retry enrollment + sync
5. Validate with Intune portal + device status screens


