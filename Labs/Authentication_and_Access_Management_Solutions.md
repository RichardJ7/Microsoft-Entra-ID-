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

4. Before I continued testing the implementation of SSPR, I had to enable phone number as an option for authentication method and SSPR for the users within the test group. I enabled this authentication for the remainder of the lab to help with the authentication and SSPR process and verification. I did this by navigating to the 'Authentication methods' section under Entra ID within the Entra ID admin center. I selected 'SMS' and enabled this authentication method for all the users within the tenant upon sign-in.  

<img width="1440" height="697" alt="SSPR pt 5" src="https://github.com/user-attachments/assets/add25b60-7e21-4584-a94a-cf8b45deafb5" />

5. After I finished configuring SSPR for this group, I needed to register SSPR and ensure that it works properly. To confirm, I opened this link, https://aka.ms/ssprsetup in a separate private browsing session to make sure that I would be required to authenticate. I then signed in using the credentials of one of the new users that I created for the SSPR Test group. I had to login using these credentials because my normal credentials provided me with the permissions of a Global Administrator. I added the phone number as an authentication method previously to the members of the test group, so using those credentials would provide me with the necessary verification. I then followed the directions on screen by first updating the password for the new user I created for the test group. Then, I selected the set up a different way option. I proceeded to input my phone number and request the text message code. Once I received the code, I finished the set up and closed the browser. 

<img width="1440" height="690" alt="SSPR pt 6" src="https://github.com/user-attachments/assets/1ade9d41-20f1-4fdc-ae74-b206b8b3260e" />

<img width="1439" height="692" alt="SSPR pt 7" src="https://github.com/user-attachments/assets/0f710c06-c768-4c7d-b018-3d42688a5f02" />

<img width="1440" height="741" alt="SSPR pt 8" src="https://github.com/user-attachments/assets/026292a1-25b3-44ec-b060-2e5bf7736b33" />

6. Since I registered the user for SSPR, I then needed to confirm if the user could reset their password. I opened this link, https://aka.ms/sspr, in another private browser. This page should appear.

<img width="1440" height="752" alt="SSPR pt9" src="https://github.com/user-attachments/assets/4daa0da7-e460-4ff2-bcac-d8679cdf6b43" />

7. I proceeded to fill out the necessary values for each verification step. Upon completion, it lead to the next page. This page gave me the option to input the phone number that is associated with the account requesting the password reset. Upon entering that, I received a verification code which I then used and now the password reset was verified. This indicates that the SSPR configuration was successful and could be implemented at a larger scale.

<img width="1430" height="781" alt="SSPR pt 10" src="https://github.com/user-attachments/assets/2e13b38e-b00c-4241-9a18-9312d449026b" />

#### Part 2: Smart Lockout Value

1. To begin this lab, I returned to the Entra Admin Center and navigated to the menu option labeled 'Authentication methods'. While there I selected 'Password Protection'.

<img width="1440" height="677" alt="Smart Lockout pt1" src="https://github.com/user-attachments/assets/5fccca12-77f6-42ed-bf53-cfd79bed7b38" />

2. I then proceeded to edit the value in the 'lockout duration in seconds' box. I changed the value from 60 seconds to 120 seconds. I then left the remainder of the settings the exact same except for the last option, which was mode. By default, that option is set to 'Audit' which only logs the attempts. By switching to enabled however, the actual values will be enforced. Once finished, I selected save and the configuration is set. This can then be tested to see if it works by incorrectly inputting the password for one of the user accounts. 

<img width="1440" height="701" alt="Smart Lockout pt2  " src="https://github.com/user-attachments/assets/802c5afc-7f92-4a09-bc2f-29921ff3ec3d" />

### Security Rationale

The reasoning behind this lab was to implement a solution that would prevent brute force attacks on user accounts. By increasing the time in between incorrect password attempts, it increases the difficulty for malicious attackers to compromise user accounts. The smart lockout value utilizes two different counters additionally, using familiar and unfamiliar locations. This helps with the mitigation of brute attacks. Hypothetically, in an organization if perhaps a user inputs an incorrect password, but it is due to a genuine forgotten password, there should be a measure in place that would help resolve this issue as quickly as possible to continue productivity and prevent downtime. That solution is a self-service password reset. This allows users who have legitimately forgotten the password to their credentials, to request a password reset through authentication methods that confirm the authenticity of the attempt. This also helps eliminate requests to the IT help desk department by providing a simple solution for forgotten credentials. 

### Lessons Learned

Through this lab, I learned how to edit the authentication methods associated with SSPR while also how to properly configure SSPR. I learned how to edit the smart lockout values to help mitigate the risk of malicious actors compromising an organization through user's credentials. 

