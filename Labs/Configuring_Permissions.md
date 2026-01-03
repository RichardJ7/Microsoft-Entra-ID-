# Configuring Permissions

## Summary 

After the new user has been created and granted a role assignment, the user's permissions can now be altered based on the role within the organization. The purpose of the lab is it improve my knowledge of user role assignments and permissions. Also, the types of permissions that are available to for customization. I will first confirm the role assignment and explore the capabilities within that role to confirm that it does not exceed scope. Then, I will explore the permissions to align with what is expected from the role that was assigned. 

## Implementation Steps

1. First, I navigated to the 'Users' section from the Entra Admin Center. After selecting this option, I proceeded to select the user that was created previously named Chris Marks.
2. Once this user's profile is selected, since I previously assigned a role for the purposes of the example, I navigated to the 'Assigned Roles' option and removed the role previously assigned.
3. After removing the previously assigned role, I assigned a new role with the settings properly configured to confirm the role operated accordingly for the purposes of the lab. I selected 'Add assignments' and then selected the 'Application administrator' role for the user Chris. I then selected 'Next' and selected the 'Active' option before providing a justification for the designation.
4. Now to confirm that the Application Administrator role is working accordingly for Chris after I assigned it, I had to utilize Chris' login through Microsoft Entra admin center. After logging in successfully with Chris' credentials, I navigated to the search bar at the top of the screen. I then searched for 'Enterprise Applications' and selected that option. A new screen appeared with the option to select 'New Application'. Once selected there should be multiple applications that can be created. This successfully verified that the role worked as intended.
5. 
