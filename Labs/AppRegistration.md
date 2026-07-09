# App Registration 

## Summary 

The purpose of an app registration is to establish a trust relationship between the application and the Microsoft identity platform. This lab shows the process of registering an application in the tenant to establish the trust relationship, thus granting identity and access management for the applications. 

### Implementation Steps

1. First, I logged into the Microsoft Entra admin center with at least the Application Developer role.
2. Under the 'Entra ID' pane, I selected the option 'App registrations'.

<img width="1440" height="685" alt="App registration pt1  " src="https://github.com/user-attachments/assets/69c8c491-8f0d-419f-bb5e-fec6c459dcb8" />

3. Next, I selected the option ‘New registration’ after the new menu appeared. 

<img width="1437" height="705" alt="App registrations pt2" src="https://github.com/user-attachments/assets/dabb6848-edf1-4eab-b1b7-fed2ed7978a6" />

4. The following page I created a name for the application registration first. Then, under the 'Supported account types' dropdown menu, I selected 'Single tenant only' option and left the 'Redirect URI' option unselected.

<img width="1438" height="669" alt="App registration pt3  " src="https://github.com/user-attachments/assets/78e9e9f9-e212-4e3e-9699-93a26158a43a" />

5. Finally, I selected 'Register' to complete the registration completion.

### Security Rationale 

Applications cannot interact with Microsoft services within the tenant or APIs without having a registration to form the trust relationship with the Entra identity platform. By creating the registration, that trust connection is established ultimately providing the ability to integrate with Microsoft securely and applying identity and access management of the application. The registration of the application allows for the configuration of certificates, secrets and assignable roles directly to the application. Additionally, the configuration of redirect URIs. 

### Lessons Learned

Through the completion of this lab, I learned how to create a registration for an application in an enterprise environment and gained familiarity with the granularities of application settings customization. 

