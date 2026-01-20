# MFA and Conditional Access

## Summary

This lab focused on configuring Multifactor Authentication and utilizing Conditional Access policies to accomplish such. This was implemented to increase the security of user login and understanding how to mitigate potential risks associated with user profiles and their access to resources within organizations.  

### Implementation Steps

#### Part 1: Enabling Multifactor Authentication

1. MFA can only be configured if either the Microsoft Entra ID P1 or P2 license is acquired. I acquired the P2 license upon the creation of this tenant with the intention of utilizing features, such as the aforementioned MFA. I first began by confirming that the feature was available which required me to first sign in to the Azure portal then navigate to the Entra ID dashboard.

<img width="1438" height="689" alt="Azure Portal " src="https://github.com/user-attachments/assets/d4dc07e2-c9a2-487a-a49d-f68e1e1f8286" />

2. After I accessed Entra ID through the Azure portal, I then proceeded to access the 'Security' tab located to the left underneath the Entra ID menu. While within 'Security', I selected the 'Manage' drop down menu which revealed the option for 'Multifactor Authentication', which was also selected.

<img width="1437" height="675" alt="Azure Portal pt2" src="https://github.com/user-attachments/assets/39cc9890-763c-412b-8bd0-8e6351cc7cfe" />

<img width="1439" height="672" alt="Azure portal pt3" src="https://github.com/user-attachments/assets/06d21ada-35c7-4982-a465-ca2b5cdf0373" />

3. Next, I accessed the option underneath 'Configure' labeled 'Additional cloud-based multifactor authentication settings' which then populated all of the available users that were in the organization.

<img width="1438" height="691" alt="MFA pt 1" src="https://github.com/user-attachments/assets/78266ebe-c4d5-414c-a477-affe4579b9f7" />

<img width="1440" height="698" alt="MFA Pt 2 " src="https://github.com/user-attachments/assets/1beb3717-e0d6-41d4-9a7a-ce632d223397" />

4. Next to the 'Users' option was the option for 'Service settings'. While within service settings, I configured the MFA settings based on how I intended the deployment to operate.

<img width="1440" height="694" alt="MFA Pt 3" src="https://github.com/user-attachments/assets/babcde79-a561-4d88-9a47-345a5d4af4a3" />

<img width="1436" height="696" alt="MFA pt 4" src="https://github.com/user-attachments/assets/7f6df477-4afa-4177-bdb9-197275424116" />

#### Part 2: Conditional Access

1. To access Conditional Access, I had to return to the Azure portal and selected Entra ID again. I then navigated to 'Security' again and while within this section, I had to find the option for Conditional Access. I found the option under the menu section titled 'Protect'. 

<img width="1429" height="670" alt="Conditional Access pt1" src="https://github.com/user-attachments/assets/752337c2-75f7-4d3b-90ad-482bd2294ae4" />

2. Now that I successfully accessed Conditional Access for the organization, I proceeded to select 'Create New Policy'. I then configured the policy accordingly to enable multifactor authentication within the organization and based on specific conditions. It should be noted that configuring Conditional Access may require the disabling of security defaults before proceeding with the establishment of the new policy. If so, follow the prompts on the screen necessary understanding that security defaults provide an enhanced security posture through preconfigured settings established through Microsoft.

