# Basic Employee Onboarding (AD)(RBAC)

## Problem Statement
Northstar Medical Group's IT environment had been managed by an external MSP with little structure or documentation, leaving day-to-day administration inconsistent and hard to maintain. User and computer accounts lacked any organizational hierarchy, with no Organizational Unit structure to support role-based management or delegation. Routine administrative tasks — account provisioning, permission changes, policy enforcement — were handled manually rather than through Group Policy, increasing the chance of inconsistent configurations. Given the sensitivity of healthcare data, this lack of structure posed a compliance risk under HIPAA, since there were no clear boundaries in place to support least-privilege access. This project rebuilds the environment from the ground up with a properly designed OU structure and Group Policy Objects to establish the organizational and administrative foundation a healthcare environment like this requires.
## Solution Overview
To address these gaps, I stood up a new Active Directory domain from scratch in Windows Server 2022, giving Northstar Medical Group a clean environment free of the previous MSP's undocumented sprawl. I designed a structured Organizational Unit hierarchy that mirrors the organization's departments and functions, enabling targeted Group Policy application and clear delegation boundaries instead of a flat, unmanaged directory. Security groups were built around a flat role-based access control model, so permissions are assigned by job function rather than to individual users, reducing the risk of excessive or inconsistent access. User provisioning was secured by tying new account creation directly to these security groups and OU placement, ensuring every new user automatically inherits the correct permissions and policy scope rather than being configured manually. Together, this rebuilds Northstar's directory services with the structure, consistency, and access control discipline that a healthcare environment needs — replacing ad hoc MSP management with a maintainable, auditable foundation.

## Tools Used
* Windows Server
* Active Directory Domain Services
* VirtualBox
* UTM
* RBAC
* GitHub

## Project Timeline
* Day 1: Domain creation and domain controller promotion
* Day 2: Organizational unit and security group design
* Day 3: User provisioning and RBAC implementation
* Day 4: Incident response and resolution (NMG-0047)
* Day 5: Documentation and case study packaging

## Key Accomplishments
* Built NMG.com domain from scratch
* [Solve the issue and double check everything looks well organized]
* [Documents the process of resolution plus screenshots of all steps from beginning to the end. ]
