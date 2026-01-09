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

1. The user Chris Marks was assigned a preconfigured role through Entra as opposed to a custom role. It should be noted that roles that are automatically created through Entra cannot have their permissions edited. To maintain least privilege, I had to ensure that the permissions for the role did not exceed the scope of the intended purpose. To verify the permissions of the Application Administrator role, I first navigated to the 'Roles & admins' section under the Entra dashboard. This then opened the 'All roles' section by default where I was able to see a list of all preconfigured roles through Entra. Next, I searched for the Application Administrator role and utilized the options feature all the way to the right of the listed role. It was labeled 'Description' which I then selected.

<img width="1440" height="697" alt="Permissions Description" src="https://github.com/user-attachments/assets/7afb2545-a799-4cb9-9848-261e5cdc1205" />

2. After, I went through the permissions of this role extensively to determine which permissions were necessary and which permissions exceeded the scope of the intended role.
3. Because the organization being used is solely for the purposes of the lab, the role of Application Administrator is currently not a necessary role now. But to display least privilege in practice, I proceeded to create a new custom role that utilized the permissions of Application Administrator but with limited permissions to prevent a potential privilege creep. I achieved this by first returning to the permissions description listed under Application Administrator and documenting all the permissions that I deemed essential for this hypothetical scenario.

<img width="1437" height="695" alt="App Admin Perm list" src="https://github.com/user-attachments/assets/243842a4-b24e-4d7a-b63b-ec83c3483fc4" />

4. Next, I returned to the 'Roles & admins' section from the Entra dashboard. I then selected the option at the top labeled 'New custom role'. I filled in the values necessary starting with 'Name' and 'Description'. Since this role is entirely fabricated for the sake of the scenario, I checked the Baseline permissions option of 'Start from scratch' because I do not have a custom role to clone it from and then proceeded by selecting 'Next' at the bottom of the screen.

<img width="1440" height="655" alt="Custom Role pt1" src="https://github.com/user-attachments/assets/7ae31228-5578-4222-a0c5-bab1179a5122" />

5. Because I read the full permission list of the actual Application Administrator role, I decided that this new custom role did not need the full extent of the permissions granted. I then selected the permissions individually that I wanted applied to the role. 
