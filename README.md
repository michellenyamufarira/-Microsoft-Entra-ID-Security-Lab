
# Enterprise Cloud Identity (IAM) & Incident Response Sandbox Lab

## Project Overview
This hands-on project demonstrates the design, deployment, and security hardening of an enterprise cloud infrastructure using **Microsoft Entra ID (Free Tier)**. The lab simulates real-world identity lifecycle management, group-based permissions structures, and an active incident response containment workflow to defend against a credential-compromise attack vector.

## Core Cybersecurity Concepts Implemented
* **Identity Lifecycle Management:** Administered secure onboarding workflows for distinct enterprise roles.
* **Principle of Least Privilege (PoLP):** Assigned granular administrative roles to limit blast radius during security events.
* **Role-Based Access Control (RBAC):** Built security group structures to standardize directory permissions profiles.
* **Incident Response & Triage:** Executed emergency isolation protocols to neutralize an active threat and contain directory breaches.

---

## Lab Architecture & Phase Breakdown

### Phase 1: Directory Architecture & User Provisioning
To mimic a corporate enterprise environment, I deployed a customized directory hierarchy consisting of targeted personnel identities and role-focused management containers:
* **Personnel Onboarded:**
  * `Kentrell ITAdmin` (IT Support Specialist / Identity Administrator)
  * `Finance Employee` (Standard Corporate End-User)
* **RBAC Infrastructure:** Established a dedicated security group named `SG-IT-Operations` to centralize permission profiles, enforcing consistent account tracking.

### Phase 2: Privileged Access Management (PAM)
To simulate administrative scaling while enforcing strict data security boundaries:
* Bypassed platform tier licensing constraints by successfully engineering direct assignment pathways for privileged roles.
* Provisioned `Kentrell ITAdmin` with **Helpdesk Administrator** directory clearances. This granted the identity required capabilities to handle password updates and user lockouts while maintaining zero access to master-level tenant configuration keys.

### Phase 3: Incident Response Simulation (Compromised Credential Triaging)
I executed an active containment drill simulating a critical SOC alert indicating an end-user identity (`Finance Employee`) suffered a dark-web credential leak. 

**The Containment Workflow Implemented:**
1. **Global Session Revocation:** Triggered an immediate session invalidation protocol to forcibly drop all active refresh tokens, cookies, and active web connections globally, neutralizing any current attacker connections.
2. **Perimeter Lockout Enforcement:** Navigated to identity attributes and systematically disabled the account (`Account Enabled = False`), freezing the directory front door and denying any subsequent login attempts regardless of credential accuracy.

---

## Skills Verified
* Cloud Directory Administration (Microsoft Entra ID)
* Identity & Access Management (IAM) Workflow Design
* Incident Response Containment Topography
* Enterprise User/Group Lifecycle Automation

## lab visual proof and & evidence
### 1. Active corporate directory setup
<img width="1354" height="588" alt="1-user-directory" src="https://github.com/user-attachments/assets/98960408-ce41-47c5-b636-e7c3d145d746" />

### 2. privileged access role assignment
<img width="1361" height="628" alt="2-privileged-access" src="https://github.com/user-attachments/assets/6730d492-04f6-4441-b7f3-c82b97fd088c" />

### 3. compromised account incident isolation (containment)
<img width="1360" height="630" alt="3-incident-containment" src="https://github.com/user-attachments/assets/70d88810-f180-4304-b60a-a96d7682abd9" />


