# Active-Directory-Domain-Services-Lab
This project demonstrates the setup and configuration of a Windows Server Active Directory environment from scratch. The goal was to simulate a real enterprise domain controller used in IT support and system administration environments.

# Objectives

- Install and configure Windows Server
- Promote server to Domain Controller
- Configure static IP addressing
- Set up Active Directory Domain Services (AD DS)
- Create and manage domain users
- Test domain authentication
- Organize users into Organizational Units and configure Group Policy
- Diagnose and resolve Group Policy application issues

# Tools Used

- Windows Server 2022
- Active Directory Domain Services
- VirtualBox
- Group Policy Management Console
- Active Directory Users and Computers

# Lab Steps Summary
1. Windows Server Setup

Installed Windows Server and completed initial configuration.

2. Network Configuration

Configured static IP address for domain controller functionality.

3. Active Directory Installation

Installed AD DS role and promoted server to a domain controller.

4. Domain Setup

Created a new forest:
**corp.local**

5. User Management

Created 3 Organizational Units (IT, Sales, HR) and 3 domain user accounts, one assigned to each OU, using Active Directory Users and Computers.

6. Authentication Testing

Successfully logged into domain using each of the three domain user accounts (IT User, Sales User, HR User) to validate authentication.

7. Group Policy Configuration

Created and linked 2 Group Policy Objects: an Account Lockout Policy (5 invalid attempts, 30-minute lockout/reset) applied to the IT OU, and a Control Panel Restriction policy applied to the Sales OU. Diagnosed and resolved a Security Filtering issue preventing GPO application, then validated enforcement — including triggering and confirming an actual account lockout — using gpresult and Active Directory Users and Computers.
 
# Screenshots
**Server Configuration**

![Server-Manager](/Screenshots/Server-Manager.png)
![SM-Local-Server](/Screenshots/SM-Local-Server.png)

**Network Configuration**

![IPv4-Properties](/Screenshots/IPv4-Properties.png)

**Active Directory Setup**

![AD-DS-install](/Screenshots/AD-DS-install.png)
![Domain-created](/Screenshots/Domain-created.png)

**User Management**

![User-created](/Screenshots/User-created.png)

**Authentication Testing**

![Domain-User-Login](/Screenshots/Domain-User-Login.png)

**Group Policy Configuration**

![OU-Structure](/Screenshots/OU-Structure.png)
![GPO-List](/Screenshots/GPO-List.png)
![Account-Lockout-Policy](/Screenshots/Account-Lockout-Policy.png)
![gpresult-Validation](/Screenshots/gpresult-Validation.png)
![Account-Locked-Screen](/Screenshots/Account-Lockout-Screen.png)
![Account-Unlocked](/Screenshots/Account-Unlocked.png)

# Key Skills Demonstrated

- Windows Server Administration
- Active Directory Management
- Domain Controller Configuration
- Network Configuration (Static IP)
- Troubleshooting Group Policy and Login Issues
- Group Policy Object (GPO) Creation and Management
- Security Filtering and Access Troubleshooting

# Outcome

A fully functional Active Directory environment was successfully deployed and tested, simulating real-world enterprise identity management.
