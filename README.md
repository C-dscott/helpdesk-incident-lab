# 🖥️ IT Help Desk Simulation — Incident Management & Troubleshooting Workflow

![Active Directory](https://img.shields.io/badge/Active%20Directory-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)
![ServiceNow](https://img.shields.io/badge/ServiceNow-00C244?style=for-the-badge&logo=servicenow&logoColor=white)
![Windows Server](https://img.shields.io/badge/Windows%20Server%202022-0078D6?style=for-the-badge&logo=windows&logoColor=white)
![VirtualBox](https://img.shields.io/badge/VirtualBox-183A61?style=for-the-badge&logo=virtualbox&logoColor=white)
![Status](https://img.shields.io/badge/Status-Active-brightgreen?style=for-the-badge)

---

## 📋 Project Overview

This project simulates a real IT Help Desk environment by generating common incident tickets through **ServiceNow** and resolving them in a **Windows Server 2022 / Active Directory** lab. Each ticket represents a task that a Help Desk Support Technician would handle on a typical workday.

Rather than simply listing skills on a resume, this project documents the complete workflow — from the moment a ticket is opened in ServiceNow through to resolution and closure — the same way it would be handled in a professional IT environment.

This lab is part of a larger portfolio that includes an **Active Directory New Employee Onboarding Lab**, together demonstrating a full picture of on-premises IT infrastructure management and Help Desk operations.

---

## 🎯 Objectives

- Simulate real Help Desk incident tickets using ServiceNow for five common IT scenarios
- Resolve each incident in Active Directory and document every step within the ticket
- Demonstrate proper ticket lifecycle — open, assign, in progress, resolve, and close
- Apply best practices for account management, password security, and access control
- Connect ServiceNow workflow to real Active Directory tasks in a virtualized environment
- Write clear, professional resolution notes within each ticket as a real technician would

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| **ServiceNow** | Incident ticket creation, routing, and closure |
| **Windows Server 2022** | Server operating system for the lab environment |
| **Active Directory Users & Computers (ADUC)** | User account and group management |
| **VirtualBox** | Hypervisor for the virtualized lab environment |
| **PowerShell** | Optional command-line administration |

---

## 🖥️ Lab Environment

```
Hypervisor     :  Oracle VirtualBox
Server OS      :  Windows Server 2022 (Desktop Experience)
Role           :  Active Directory Domain Services (AD DS)
Domain         :  carolyn.org
Ticketing      :  ServiceNow (Developer Instance)
OU Structure   :  ITCorp > HR | IT | Sales | Disabled Users
```

---

## ✅ Skills Demonstrated

- **ServiceNow ITSM** — Creating, categorizing, prioritizing, routing, and closing incident tickets
- **Account Lockout Resolution** — Identifying locked accounts in ADUC and unlocking with proper documentation
- **Password Reset** — Resetting user passwords and enforcing best practice security policies
- **Security Group Management** — Adding users to Security Groups to grant access to shared resources
- **Account Deprovisioning** — Disabling terminated employee accounts and moving to Disabled Users OU
- **Account Property Updates** — Correcting user display names and account attributes in Active Directory
- **Ticket Documentation** — Writing professional resolution notes and maintaining ticket lifecycle records

---

## 🎫 Incident Tickets

The following five incidents were created in ServiceNow and resolved in Active Directory. Each ticket simulates a real Help Desk scenario.

| Ticket # | Issue | Affected User | Priority | Status |
|----------|-------|---------------|----------|--------|
| INC-0010023 | Account lockout — user cannot log in | Barry Harriston | 🔴 High | ✅ Resolved |
| INC-0010024 | Forgotten password — reset required | Carli Trueblood | 🟡 Standard | ✅ Resolved |
| INC-0010025 | New employee needs shared folder access | Joane Ausherman | 🟡 Standard | ✅ Resolved |
| INC-0010026 | Terminated employee — disable account immediately | Mark Cogswell | 🔴 High | ✅ Resolved |
| INC-0010027 | Incorrect display name in Active Directory | Rowena Steeves | 🟡 Standard | ✅ Resolved |

---

## 📂 Step-by-Step Walkthrough

Each incident followed the same professional workflow from start to finish:

### Step 1 — Ticket Created in ServiceNow
The incident was logged in ServiceNow with a title, description, affected user, priority level, and assignment to the IT Help Desk group.

### Step 2 — Ticket Assigned & Set to In Progress
The ticket was assigned to the technician and the status was updated to **In Progress** before any work began, reflecting real-world ticketing best practices.

### Step 3 — Issue Resolved in Active Directory
The technical task was performed in Active Directory Users and Computers. Depending on the ticket this included unlocking an account, resetting a password, updating Security Group membership, disabling an account, or correcting account properties.

### Step 4 — Resolution Notes Documented in Ticket
A clear, professional resolution note was added to the ticket explaining exactly what action was taken, when it was completed, and any follow-up steps required.

### Step 5 — Ticket Closed
The ticket status was updated to **Resolved** and then **Closed**, completing the full incident lifecycle in ServiceNow.

---

## 🔍 Ticket Details & Resolution Notes

---

### 🎫 INC-0010023 — Account Lockout

**Affected User:** Barry Harriston
**Priority:** High
**Category:** Account Management

**Issue Description:**
User Barry Harriston called the Help Desk reporting he could not log in to his workstation. He received an error message stating his account was locked.

**Resolution:**
Located Barry Harriston's account in Active Directory Users and Computers. Confirmed the account was locked out on the Account tab. Verified the identity of the caller before proceeding. Unlocked the account and reset the temporary password to Welcome1! with the requirement to change at next logon. Confirmed with the user that she was able to log in successfully.

**Resolution Time:** 8 minutes
**Status:** Closed

---

### 🎫 INC-0010024 — Password Reset

**Affected User:** Carli Trueblood
**Priority:** Standard
**Category:** Password Management

**Issue Description:**
User Carli Trueblood submitted a ticket stating she forgot her password and could not log in to her account.

**Resolution:**
Located Carli Trueblood's account in Active Directory Users and Computers. Verified the identity of the user before proceeding. Reset the password to the temporary password Welcome1! and checked the box requiring the user to change her password at next logon. Notified the user of the temporary password via phone. Confirmed the user was able to log in and set a new password successfully.

**Resolution Time:** 5 minutes
**Status:** Closed

---

### 🎫 INC-0010025 — Shared Folder Access Request

**Affected User:** Joane Ausherman
**Priority:** Standard
**Category:** Access Management

**Issue Description:**
New employee Joane Ausherman submitted a ticket reporting she was unable to access the Sales department shared network folder needed to perform her job duties.

**Resolution:**
Located Joane Ausherman's account in Active Directory Users and Computers. Navigated to the Member Of tab in her account properties. Added her account to the Sales_Team Security Group which controls access to the Sales shared folder. Confirmed the group membership was saved. Notified Joane that access had been granted and asked her to log out and back in for the changes to take effect. User confirmed access was working.

**Resolution Time:** 6 minutes
**Status:** Closed

---

### 🎫 INC-0010026 — Terminated Employee Account Disable

**Affected User:** Mark Cogswell
**Priority:** High
**Category:** Account Deprovisioning

**Issue Description:**
HR submitted an urgent ticket requesting the immediate disabling of Mark Cogswell's account following his termination effective end of business today.

**Resolution:**
Located Mark Cogswell's account in Active Directory Users and Computers. Right-clicked the account and selected Disable Account. Confirmed the account showed a disabled indicator. Removed the account from all Security Groups to revoke resource access. Moved the disabled account to the Disabled Users OU for retention per company policy. Account will be reviewed for permanent deletion after the standard 90-day retention period. Notified HR that the account had been disabled and all access revoked.

**Resolution Time:** 10 minutes
**Status:** Closed

---

### 🎫 INC-0010027 — Incorrect Display Name

**Affected User:** Rowena Steeves
**Priority:** Standard
**Category:** Account Maintenance

**Issue Description:**
User Rowena Steeves submitted a ticket reporting that her display name was appearing incorrectly in the company directory and in Microsoft Outlook. Her name was showing as Rowena Steenes instead of Rowena Steeves.

**Resolution:**
Located Rowena Steeves's account in Active Directory Users and Computers. Opened her account properties and navigated to the General tab. Updated the Last Name field from Steenes to Steeves and confirmed the Display Name field updated accordingly. Saved the changes. Notified the user that the correction had been made and that the update would reflect in the directory and Outlook within the standard replication window.

**Resolution Time:** 4 minutes
**Status:** Closed

---

## 📸 Screenshots



ServiceNow ticket detail — INC- 0010023 account lockout 
<br /> Account Lockout - Ticket Details <br/>
<img src="https://imgur.com/KAj4e1M.png" height="80%" width="80%" alt="Creating Ticket Reference Steps"/>
<br />
<br />
Active Directory — unlocking a locked account 
<br />
<img src="https://imgur.com/oBIAu8Z.png" height="80%" width="80%" alt="Creating Ticket Reference Steps"/>
<br />
<img src="https://imgur.com/6YuwC86.png" height="80%" width="80%" alt="Creating Ticket Reference  Steps"/>
<br />
<img src="https://imgur.com/QDdUBK4.png" height="80%" width="80%" alt="Creating Ticket Reference  Steps"/>
<br />
<img src="https://imgur.com/DvUS3Hh.png" height="80%" width="80%" alt="Creating Ticket Reference  Steps"/>
<br />
<img src="https://imgur.com/OVH8jc3.png" height="80%" width="80%" alt="Creating Ticket Reference Steps"/>
<br />
<br />
Active Directory — Security Group membership update 
<br /> Security Group Update  <br/>
<img src="https://imgur.com/qDHloDX.png" height="80%" width="80%" alt="Disabling the Account Steps"/>
<br />
<br />
Active Directory — disabled account in Disabled Users OU 
<br /> Disabling the Account — Employee Offboarding  <br/>
<img src="https://imgur.com/LEHHgDD.png" height="80%" width="80%" alt="Disabling the Account Steps"/>
<br />
<img src="https://imgur.com/oRK6BZs.png" height="80%" width="80%" alt="Disabling the Account Steps"/>
<br />
<img src="https://imgur.com/kL1DuX5.png" height="80%" width="80%" alt="Disabling the Account Steps"/>
<br />
<img src="https://imgur.com/1s5FFL7.png" height="80%" width="80%" alt="Disabling the Account Steps"/>
<br />
<img src="https://imgur.com/lIX5eqT.png" height="80%" width="80%" alt="Disabling the Account Steps"/>
<br />
<br />
ServiceNow — closed ticket with resolution notes 
<br /> Closed Ticket  <br/>
<img src="https://imgur.com/2yajfJr.png" height="80%" width="80%" alt="Disabling the Account Steps"/>
<br />
---

## 🎥 Video Walkthrough

A full video walkthrough of this lab is available on YouTube. Watch the complete workflow from ticket creation in ServiceNow through to resolution and closure in Active Directory.

▶️ **[Watch on YouTube](https://www.youtube.com/playlist?list=PLoowYzuxGQ0AnRZMVtwsAvOnVTKLQKhEM)**

---

## 🔗 Related Projects

This lab is part of a growing IT Help Desk portfolio:

| Project | Description |
|---------|-------------|
| [Active Directory Lab #1 — New Employee Onboarding](https://github.com/C-dscott/ActiveDirectoryLab#active-directory-home-lab) | Full employee account lifecycle — onboarding through offboarding |
| **IT Help Desk Simulation — Incident Management** *(This Repo)* | Five real-world incident tickets created in ServiceNow and resolved in Active Directory |

---

## 💡 Key Takeaways

This lab reinforced that the technical task is only half of the Help Desk job. Knowing how to unlock an account or reset a password is important — but documenting it clearly, updating the ticket at every stage, and closing it properly is what separates a good technician from a great one.

Working through these five scenarios gave me a real appreciation for how ServiceNow connects the entire IT workflow from the moment a user reports a problem to the moment it is fully resolved. That full-cycle visibility is something I look forward to bringing to a real Help Desk team.

---

## 📬 Connect With Me

I am actively seeking my first IT Help Desk Support role. Feel free to reach out — I would love to connect.

- 💼 **[LinkedIn](https://www.linkedin.com/in/carolynscott55/)**
- 🐙 **[GitHub](https://github.com/C-dscott)**
  

---

*This project is part of a growing IT portfolio. More labs coming soon.*
