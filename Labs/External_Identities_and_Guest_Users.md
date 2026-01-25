# External Identities and Guest Users

## Summary

The purpose of the lab was to configure external collaboration within the tenant and the implementation of guest users. I documented the process of how I configured these external identities, including their access to resources within the tenant. 

## Implementation Steps

### Part 1: Configuring External Collaboration

1. To begin this lab, I signed into the Entra admin center. Once there, I navigated to the menu on the left under Entra ID and selected 'External Identities'. I then selected the 'External Collaboration Settings' option within 'External Identities'.

<img width="1434" height="702" alt="External Collab pt1" src="https://github.com/user-attachments/assets/c81bcb9c-cde6-40d4-8a92-da64528d5715" />

<img width="1440" height="706" alt="External Collab pt2" src="https://github.com/user-attachments/assets/2c48d04b-112d-4369-8252-be3ca071403a" />

2. Next, I had the option to configure the settings accordingly based on how I intended these users to operate within the tenant. I did not want these guest users to have similar access and permissions as members that are within the internal organization, so I opted to designate the most restrictive settings for these users. Once finished, I saved the changes to apply to the tenant.

<img width="1440" height="696" alt="External Collab pt3" src="https://github.com/user-attachments/assets/83b11ca9-c47b-4735-bed9-d1b89d4def9b" />

<img width="1439" height="697" alt="External Collab pt4" src="https://github.com/user-attachments/assets/adc0c291-c6f3-4c25-abf7-5f39eb7b2e13" />

### Part 2: Adding Guest Users

1. While within the admin center, I navigated back to the 'Users' section of the Entra ID menu. Once there, I selected 'New user' which gave me the option to decide between creating a new user or inviting an external user. I chose the latter.

<img width="1440" height="701" alt="Guest User pt1" src="https://github.com/user-attachments/assets/6be74eb3-870c-4d79-98ec-382cf4cf9e34" />

2. Since I do not have an actual external organization collaborating with me for this lab, I input the necessary values into the field using my own information to send an invitation as the external guest user. There is an option to confirgure properties and assignments once the first page is completed, but I will not need to configure any of those settings because this guest user will not have a role.

<img width="1440" height="701" alt="guest user pt2" src="https://github.com/user-attachments/assets/917f0298-8e62-4f2d-b589-35765efe89e3" />

3. I wanted to confirm that the guest user was successfully added and had the guest designation under user type, so I returned to the guest menu and refreshed the directory to ensure that I successfully added.

<img width="1440" height="696" alt="guest user pt3" src="https://github.com/user-attachments/assets/68232263-1e73-4eb9-9ce0-a06f1275ad54" />

## Security Rationale

There would be instances that a tenant would need to add collaborators outside of the organization. These collaborators however could not have permissions and access that are comparable to an internal user. I configured the external users and guest to have access to the resources of the organization but without any privileged or administrative responsibilities. 

## Lessons Learned

This lab helped me improve how to identify the role of guest users within the tenant. Additionally, it helped me with familiarizing myself with how to create an external identity and adjust the initial settings to create a restricted guest user. 
