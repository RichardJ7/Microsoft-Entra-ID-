# Access Management For Apps

## Summary 

In enterprise environments, applications are deployed for members of the organization to access and utilize for daily operations. This lab displays how access to applications can be managed, ultimately replicating an enterprise environment that restricts access to certain applications based on the user or group's role in the enterprise. 

### Implementation Steps

#### Part 1: Adding an Application

1. Before the access rights can be managed for an application, the application must be available in the environment. First, sign-in to the Entra ID admin center and select enterprise apps.

<img width="1440" height="687" alt="Access Management Apps pt1  " src="https://github.com/user-attachments/assets/906ed979-611b-4ec6-97a9-82a9b8e52878" />

2. Next, while within enterprise applications, select the option 'New Application'.

<img width="1438" height="703" alt="App Management pt2  " src="https://github.com/user-attachments/assets/6fe56b93-9be4-4aff-9dbc-128e07a033b2" />

3. Now a new pane should appear with a search bar. In the search bar, search for 'GitHub Enterprise Cloud- Enterprise Account' and then select 'Create' once settings are reviewed.

<img width="1440" height="702" alt="App management pt 3  " src="https://github.com/user-attachments/assets/31851144-e3c8-4411-b41f-6d7b126324c8" />

#### Part 2: Managing Access

1. After the application is created, there should be a redirection to the GitHub Enterprise Cloud application overview page. There is a section on the overview page titled 'Getting Started'. Select 'Assign users and groups'.

<img width="1440" height="707" alt="App management pt 4  " src="https://github.com/user-attachments/assets/8bd8c32b-1428-4487-8ab0-a349cbe0fa3d" />

2. Then, the next pane displays the option 'Add user/group'. Select this option and then select 'None Selected' under 'Users and groups' to assign the users to the app.

<img width="1439" height="706" alt="App management pt5  " src="https://github.com/user-attachments/assets/1033d82e-7f38-4660-82d4-e4e25c886f82" />

3. Finally, select the users to be assigned access to the app and then select 'Assign' to finalize the assignment.

### Security Rationale 

In large organizations, certain applications are available to certain individuals. Some users should be permitted to access certain apps and are assigned appropriate permissions. When creating applications in the tenant, it is useful to assign specific groups or individuals with access to specific applications based on their role to prevent privilege creep or unnecessary access to applications. 

### Lessons Learned

Through the process of this lab, I was able to learn how to effectively assign specific users access to apps. I gained the ability to manage effectively user's access to apps from the overview page after creating an application. I also gained an understanding of how to add users to a particular application through the 'Enterprise App' blade and selecting the application I chose to grant access to. 



