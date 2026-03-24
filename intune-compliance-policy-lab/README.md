## Lab 2 – Windows 10/11 Compliance Policy

### Actions Performed
- Created Windows 10/11 compliance policy
- Configured noncompliance action:
  - Mark device noncompliant (Immediately)
- Assigned policy to All devices
- Avoided destructive actions (retire/wipe)

### Validation
- Windows 11 VM evaluated policy successfully
- Device status shows **Compliant** in Microsoft Intune
- Policy applied without errors or conflicts

### Device Compliance Status in Intune

![Device Compliance Status](intune-device-compliance-status.png)

This screenshot shows the Windows 11 device successfully enrolled in Microsoft Intune and marked as **Compliant** after policy evaluation.

Key details:
- Device is managed by Intune
- Compliance status = Compliant
- OS version visible
- Last check-in confirms active communication with Intune
