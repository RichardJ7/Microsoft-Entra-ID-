# Managing Lifecycle of External Users

## Summary

Oftentimes, external users will be invited to collaborate on projects or share resources with users within a tenant. They can be invited to access these resources through the use of access packages. This lab demonstrates how to effectively manage the lifecycle of these external users who were invited through access packages.

### Implementation Steps

1. First, I began by signing in to the tenant and navigating to the dashboard labeled 'ID Governance'.

2. After, I selected the option labeled 'Entitlement management' and once the menu for entitlement management opened, I selected 'Control configurations'. 

<img width="1439" height="689" alt="External Identities Lifecycle pt1" src="https://github.com/user-attachments/assets/cd8d7707-96ce-4e4c-b092-6dc46f8d52b1" />

3. Next, I selected 'View settings' under the 'Lifecycle of external users' option.

4. While these settings are now open, I configured the settings appropriately, which determines what occurs to an external user's account once they lose access to their last access package assignment. I selected 'Remove external user', 'Block external user from signing in to directory' and I selected 35 days as the 'Number of days before removing external user from directory'. Then selected save to apply these settings to the lifecycle of external users who received access through an access package request.

 <img width="1440" height="708" alt="External identities lifecycle pt2  " src="https://github.com/user-attachments/assets/916f0109-c360-4533-91a8-b30068ae4468" />

 ## Security Rationale

When an external user is finished collaborating or using resources in another tenant, they should be restricted from continued access to these resources. They should not be allowed to access the resources or the directory once they lose their last assignment to access packages. Additionally, the user's account should remain visible to administrators for auditing purposes which is why the lifecycle of the external users' accounts is important. By not restricting access, the external users' access can exceed beyond what the intended scope of their role is, ultimately jeopardizing the security of the tenant. 

## Lessons Learned

This lab provided me with necessary knowledge in managing the lifecycle of external users that are granted access to resources through access package requests. I learned how to configure the settings for external users once assignment to their last access package expires and what becomes of their account in the directory. 



