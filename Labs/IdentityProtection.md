# Summary 

This lab focused on the Microsoft Entra ID feature Identity Protection. Identity Protection was designed to monitor, detect and remediate risks related to identity. Through the monitoring of a logins, Identity Protection provides the ability to customize policies based on identity risks. In this lab, I configured two different policies to implement in an environment to mitigate identity risks related to sign-ins and users. At the time of this lab, Identity Protection User Risk Policy and Sign-in Risk Policy is now in read-only mode. I documented the process of creating these policies from the Identity Protection menu dashboard to show my familiarity with the environment. These can be configured through Conditional Access currently and can only be done after disabling Security Defaults. My proceedeing Conditional Access labs will document these policies from that dashboard. 

## Implementation Steps

### Part 1: User Risk Policy

1. I began by logging into the Entra admin dashboard and navigating directly to the section under the left menu blade titled 'ID Protection'. While there, I opened the 'Dashboard' and from within that menu section, I saw another section labeled 'Protect' which listed two different options, user risk policy and sign-in risk policy.

<img width="1440" height="679" alt="User Risk Policy pt1" src="https://github.com/user-attachments/assets/25254866-523d-41a3-88e6-21f28df55df9" />

2. The first policy I chose to configure was User risk. I selected this option while within the 'Protect' dashboard. After selecting user risk under 'Assignments', I configured the 'users' option. I selected a small number of users to include in this policy because it is generally in good practice to test the rollout of the intended policy changes before implenting them to the entire tenant to see how the environment responds to these changes.

<img width="1440" height="712" alt="User Risk Policy pt2" src="https://github.com/user-attachments/assets/c3d30751-aea2-48d3-a9ba-29e3003fafef" />

<img width="1440" height="711" alt="User Risk Policy pt3" src="https://github.com/user-attachments/assets/ad4c01e8-1b28-482e-8242-0e2f598600c4" />

3. After designating the users for the rollout of the policy, I proceeded to configure the 'User Risk' controls. By default, this option is labeled with 'Low and above' and once selected a new pane appears. It is from that new pane that I selected the control of 'High' and then selected 'Done' to proceed with the next condition to be configured. 

<img width="1440" height="708" alt="User Risk Policy pt4  " src="https://github.com/user-attachments/assets/694c990c-b432-4967-a056-cf7ff19b7326" />

4. The last condition under 'Controls' also opened a new pane which allowed me to select the Access enforcement. I selected 'Allow access' and also checked the box underneath labeled 'Require password change' and confirmed it updated once I selected 'Done' at the bottomn of the pane.

<img width="1440" height="710" alt="User Risk Policy pt5" src="https://github.com/user-attachments/assets/79a73ad1-d891-4b82-9613-6827daedc45a" />




