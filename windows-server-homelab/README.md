# 🖥️ Windows Server HomeLab (Active Directory Environment)

## 📌 Objective

The purpose of this lab was to build and configure a Windows Server environment to simulate a real-world enterprise network.

This includes setting up Active Directory, DNS, DHCP, Group Policy, and domain-joined client machines.

---

## 🧩 Scenario

A small business requires a centralised IT infrastructure to manage users, devices, and network services.

As the IT Administrator, I was responsible for building and configuring a Windows Server environment to support authentication, device management, and network services.

---

## 🛠️ Technologies Used

- Windows Server (2019 / 2022)
- Windows 10/11 Client VM
- Hyper-V (Virtualisation)
- Active Directory Domain Services (AD DS)
- DNS
- DHCP
- Group Policy (GPO)

---

## ⚙️ What I Configured

### 1. Active Directory Domain Services (AD DS)
- Installed AD DS role
- Promoted server to Domain Controller
- Created a new domain

---

### 2. User & Group Management
- Created user accounts
- Created security groups
- Assigned users to groups
- Applied basic organisational structure (OUs if used)

---

### 3. DNS Configuration
- Configured DNS as part of AD DS setup
- Verified name resolution within the domain
- Tested connectivity between machines

---

### 4. DHCP Setup
- Configured DHCP scope
- Assigned IP address ranges
- Verified client machines receive IP automatically

---

### 5. Group Policy (GPO)
- Created and applied Group Policies
- Enforced system settings (e.g. password policies, security settings)
- Tested policy application on client machines

---

### 6. Domain Join
- Joined Windows 10/11 client machine to domain
- Logged in using domain credentials
- Verified communication with Domain Controller

---

## ✅ Results

- Domain Controller successfully deployed  
- Users and groups managed through Active Directory  
- Client machine successfully joined to domain  
- DHCP assigned IP addresses correctly  
- DNS resolution working within the network  
- Group Policies applied successfully  

---

## 📸 Evidence

Screenshots included in this repository demonstrate:

- Active Directory Users and Computers  
- Domain Controller setup  
- DHCP configuration  
- Group Policy settings  
- Domain-joined client machine  

---

## 🧠 Key Skills Demonstrated

- Windows Server Administration  
- Active Directory Management  
- Networking Fundamentals (DNS, DHCP)  
- Group Policy Configuration  
- Domain Environment Setup  
- Troubleshooting Client-Server Communication  

---

## 📚 What I Learned

- How enterprise networks are structured using Active Directory  
- The role of DNS and DHCP in network functionality  
- How Group Policy enforces organisational standards  
- How to manage users and devices centrally  
- How to troubleshoot domain-related issues  

---

## 🚀 Real-World Relevance

This lab reflects core responsibilities of:

- IT Support Engineers  
- System Administrators  
- Service Desk Engineers  

Active Directory environments are still widely used in organisations, making these skills essential for IT roles.
