# Authentication and Access Management Solutions

## Summary

This lab was created to provide two common solutions that aid in protecting the identities or credentials of users. Both solutions contribute to the overall posture of an organization relative to authentication and access management solutions. The two solutions included are SSPR or self-service password reset and smart lockout values. 

### Implementation Steps

#### Part 1: Self Service Password Reset (SSPR)

1. Note that to complete this lab, SSPR can only be enabled with the purchase of a either a Microsoft Entra ID Premium P1, P2, Microsoft Business Standard or Business Premium license. This is contingent on if the user that I enabled SSPR for has an on-premises account or a cloud-based account. I purchased a P2 license upon creation of the tenant, so I was capable of completing this lab.
2. When implementing changes that can affect the entirety of the tenant, there is the potential that these changes can disrupt the environment. To ensure that the environment is not negatively affected, I created a group and a few additional users to test the SSPR.

<img width="1440" height="696" alt="SSPR pt1" src="https://github.com/user-attachments/assets/c71d2357-0030-4ae7-a4ac-c0f591fd0d24" />

<img width="1438" height="692" alt="SSPR pt 2" src="https://github.com/user-attachments/assets/429d69a5-0be3-40f7-855f-915c62e65725" />

3. After, I created the new group with the users, I then navigated to the 'password reset' option underneath the Entra ID dashboard. The option for 'self-service password reset' was initially selected as none. I changed this option to 'selected' and then added the group that I created to test SSPR. Once I selected the group, I saved the changes I made to confirm that the settings for the group were applied.

<img width="1440" height="701" alt="SSPR pt 3" src="https://github.com/user-attachments/assets/745f2796-44d8-4171-8aed-e2d3ec9d743c" />

<img width="1440" height="702" alt="SSPR pt  4" src="https://github.com/user-attachments/assets/c3f3b3a3-5bb8-4b56-b742-db2af518137e" /> 

4. After I finished configuring SSPR for this group, I needed to register SSPR and ensure that it works properly. To confirm I opened this link, https://aka.ms/ssprsetup in a separate private browsing session to make sure that I would be requried to authenticate. 
