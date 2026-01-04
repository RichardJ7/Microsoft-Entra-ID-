# Configuring Permissions

## Summary 

After the new user has been created and granted a role assignment, the user's permissions can now be altered based on the role within the organization. The purpose of the lab is it improve my knowledge of user role assignments and permissions. Also, the types of permissions that are available to for customization. I will first confirm the role assignment and explore the capabilities within that role to confirm that it does not exceed scope. Then, I will explore the permissions to align with what is expected from the role that was assigned. 

## Implementation Steps

#### Part 1: Role Assignment and Verification

1. First, I navigated to the 'Users' section from the Entra Admin Center. After selecting this option, I proceeded to select the user that was created previously named Chris Marks.
2. Once this user's profile is selected, since I previously assigned a role for the purposes of the example, I navigated to the 'Assigned Roles' option and removed the role previously assigned.
3. After removing the previously assigned role, I assigned a new role with the settings properly configured to confirm the role operated accordingly for the purposes of the lab. I selected 'Add assignments' and then selected the 'Application administrator' role for the user Chris. I then selected 'Next' and selected the 'Active' option before providing a justification for the designation.

<img width="1440" height="697" alt="Assignment Justification" src="https://github.com/user-attachments/assets/fd6dda93-4aae-40bd-8b54-484477df7703" />

4. Now to confirm that the Application Administrator role is working accordingly for Chris after I assigned it, I had to utilize Chris' login through Microsoft Entra admin center. After logging in successfully with Chris' credentials, I navigated to the search bar at the top of the screen. I then searched for 'Enterprise Applications' and selected that option. A new screen appeared with the option to select 'New Application'. Once selected there should be multiple applications that can be created. This successfully verified that the role worked as intended.

<img width="1440" height="693" alt="Role Verify1" src="https://github.com/user-attachments/assets/6a7846bb-dd4e-4469-a2ae-ea7abf2d4316" />

<img width="1436" height="695" alt="Role Verify 2" src="https://github.com/user-attachments/assets/2a993ae3-9de5-462f-85b0-8251ab6c669b" />

<img width="1440" height="696" alt="Role Verify3" src="https://github.com/user-attachments/assets/cdb2a536-b8c0-4140-8686-40b4937ba22a" />

#### Part 2: Configuring Permissions

1. 

