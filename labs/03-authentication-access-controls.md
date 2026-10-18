# Lab: User Authentication & Access Controls (Active Directory)

**Tools:** Windows Server, Active Directory Users and Computers, NTFS permissions, SMB shares

## What I did
- Created users and **security groups** in Active Directory (HR, Managers, Developers).
- Built department folders (HRfiles, MGRfiles, DEVfiles) and set **NTFS permissions per group**, following least privilege.
- Created an **SMB share** and configured share-level ACLs on top of the NTFS permissions.
- Verified the setup by logging in as different users. Each one could reach only their own department's folder and got "access denied" everywhere else. I also checked file ownership on files each user created.
- Completed the challenge: built a new set of users, groups and ACLs from scratch without step-by-step instructions.

## Takeaway
Assign permissions to **groups, not individual users**, and then test them by logging in as each role.
