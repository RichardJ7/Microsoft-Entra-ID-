# User Creation

## Summary

After the initial setup of Microsoft Entra ID and the operating organization for the ensuing labs, the first task is creating a user through Entra ID. 

## Implementation Steps

1. Sign in to Azure utilizing the organization account as the Global Administrator.
2. Navigate to the menu on the left side of the screen and press the drop down menu button labeled Entra ID. There should be multiple options once expanded. Click on the Users section.
3. On this page, select the new user button and then select create new user.
4. Begin inputting the required information starting with 'User principal name', 'mail nickname' which has included a box titled 'derived from user principal name'. Uncheck that box and put the complete mail nickname. Then, input 'display name' and 'password'. This password will not be automatically generated so that option can also be unchecked.
5. Next, select review+create. The following screen should prompt another create option which will also be selected. The new user should now be present in the organization.
6. Navigate to the 'Users' section under the Entra menu and then select 'All Users'. The new created user may not appear immediately so refresh the page. Once the user appears, select the user's profile.
7. A new menu will appear underneath the user's profile with options similar to the Entra menu under the tenant. Select the option 'Assigned Roles'

