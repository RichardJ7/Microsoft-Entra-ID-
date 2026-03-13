# Identity Protection

## Summary 

This lab focused on the Microsoft Entra ID feature Identity Protection. Identity Protection was designed to monitor, detect and remediate risks related to identity. Through the monitoring of logins, Identity Protection provides the ability to customize policies based on identity risks. In this lab, I configured two different policies to implement in an environment to mitigate identity risks related to sign-ins and users. At the time of this lab, Identity Protection User Risk Policy and Sign-in Risk Policy were in the process of being retired and thus were in read-only mode. I documented the process of creating these policies from the Identity Protection menu dashboard to show not only my familiarity with the environment but also the necessary conditions that need to be configured to create these policies to address these risks. These policies can be configured through Conditional Access currently, which can be done after disabling Security Defaults. I will explore Conditional Access in future labs. 

### Implementation Steps

#### Part 1: User Risk Policy

1. I began by logging into the Entra admin dashboard and navigating directly to the section under the left menu blade titled 'ID Protection'. While there, I opened the 'Dashboard' and from within that menu section, I saw another section labeled 'Protect' which listed two different options, user risk policy and sign-in risk policy.

<img width="1440" height="679" alt="User Risk Policy pt1" src="https://github.com/user-attachments/assets/25254866-523d-41a3-88e6-21f28df55df9" />

2. The first policy I chose to configure was User risk. I selected this option while within the 'Protect' dashboard. After selecting user risk under 'Assignments', I configured the 'users' option. I selected a small number of users to include in this policy because it is generally in good practice to test the rollout of the intended policy changes before implementing them to the entire tenant to see how the environment responds to these changes.

<img width="1440" height="712" alt="User Risk Policy pt2" src="https://github.com/user-attachments/assets/c3d30751-aea2-48d3-a9ba-29e3003fafef" />

<img width="1440" height="711" alt="User Risk Policy pt3" src="https://github.com/user-attachments/assets/ad4c01e8-1b28-482e-8242-0e2f598600c4" />

3. After designating the users for the rollout of the policy, I proceeded to configure the 'User Risk' controls. By default, this option is labeled with 'Low and above' and once selected a new pane appears. It is from that new pane that I selected the control of 'High' and then selected 'Done' to proceed with the next condition to be configured. 

<img width="1440" height="708" alt="User Risk Policy pt4  " src="https://github.com/user-attachments/assets/694c990c-b432-4967-a056-cf7ff19b7326" />

4. The last condition under 'Controls' also opened a new pane which allowed me to select the Access enforcement. I selected 'Allow access' and also checked the box underneath labeled 'Require password change' and confirmed it updated once I selected 'Done' at the bottom of the pane.
5. I finalized the policy by selecting 'Enable' under 'Policy enforcement' and then 'Save' to ensure that the policy settings were established and the policy was created. 

<img width="1440" height="710" alt="User Risk Policy pt5" src="https://github.com/user-attachments/assets/79a73ad1-d891-4b82-9613-6827daedc45a" />

#### Part 2: Sign-in Risk Policy 

1. From within the Identity Protection dashboard, I selected the option 'Sign-in risk policy' similarly to how I started the process of creating the user risk policy. The first condition that needed to be established was the assignments. I selected the users that would be included in this policy.

<img width="1440" height="689" alt="Sign-in risk policy pt1" src="https://github.com/user-attachments/assets/c56dcbe9-481c-476b-8ba5-72632170a646" />

2. Next, I configured the 'Sign-in risk' condition. In the proceeding pane that opened after selecting the 'Sign-in risk' option, I selected the control that would be enforced. I selected 'Medium and above' and selected 'Done' to confirm the selection.

<img width="1440" height="711" alt="Sign-in risk policy pt2" src="https://github.com/user-attachments/assets/f31e1ace-6924-4f55-8e2f-e808f380636b" />

3. After, I selected the controls that enforce the access. Under the 'Controls' option I selected 'Allow access' and then checked the box underneath labeled 'Require multifactor authentication'. I confirmed the selection again with 'Done'.

<img width="1440" height="711" alt="Sign-in risk policy pt3  " src="https://github.com/user-attachments/assets/49bbaf3e-8c16-4100-8fbb-a13da3bf4e11" />

4. To complete the policy, I selected 'Enable' for the 'Policy enforcement' designation and then 'Save'. 

### Security Rationale

To help remediate and respond to risks associated with identity, I wanted to ensure there were proper policies in place that would help identify suspicious activity. The cloud presents an extremely vulnerable security risk for threat actors. Threat actors have the ability to compromise multiple systems and access sensitive information by either stealing login credentials of Entra users or exploiting systems to gain unauthorized access through sign-in methods. In large environments, it is difficult to keep track and remediate all risks while actively maintaining the security of the organization. With these two policies, automated responses can be implemented to improve the posture of the organization. 

### Lessons Learned

This lab helped me to understand the conditions that are necessary when configuring policies that are directed toward remediating two different identity related risks. Since these two policies will no longer be accessible via their respective policy options under ID Protection, I also needed to get a firm grasp on what I would need to know when creating these policies from a blank starting point within Conditional Access. By exploring the conditions and seeing how these responses to suspicious activity can be effectively automated accordingly, I gained a foundational understanding that I can now apply with granularities to provide greater control over large environments. 
