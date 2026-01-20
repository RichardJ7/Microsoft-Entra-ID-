# Group Creation and Licenses

## Summary

This lab was intended to exemplify the ability to create groups within Microsoft Entra. There are two different groups that can be created within Entra, Security and Microsoft 365. In this lab, I documented the creation of both group types within Entra but also, utilized the group licensing feature and assigned licenses to the configured groups. I document how licenses can be applied to individual users or assigned directly to groups. 

## Implementation Steps 

### Part 1: Group Creation

1. I began by first creating a Microsoft 365 group. To create this group, I had to navigate to the Entra admin center. I then selected the option labeled 'New Group' and I began to complete the required fields to satisfy the completion of the group.

<img width="1439" height="693" alt="Create New Group" src="https://github.com/user-attachments/assets/191d7319-8979-4315-a282-7a3f1eb87743" />

<img width="1440" height="698" alt="Create 365 Group" src="https://github.com/user-attachments/assets/36eaaa7f-912d-4af3-a4a8-facc2ebc0c22" />

2. At the bottom of the 'New Group' field, there were two additional options. The first, option was titled 'Owners' and the second option was titled 'Members'. I proceeded to select the 'Owners' field and designated myself as the Owner since I am currently the Global Administrator of the organization. After, I designated myself as the owner, I added the previous user that I created to the group.

<img width="1434" height="588" alt="Add Group Owner " src="https://github.com/user-attachments/assets/cce858ab-2674-4355-909c-229a62eb7354" />

<img width="1440" height="698" alt="Add User to Group" src="https://github.com/user-attachments/assets/9f2d3de6-3f23-4c00-b861-83fd0f26c0d3" />

3. Because I started with the Microsoft 365 group, I then began to replicate the group creation process however, this time I created a security group that will have different roles and users. Additionally, I created two other users to add to this group to differentiate between roles and to simplify the remainder of the lab that included group licensing assignments.

<img width="1439" height="696" alt="Create Security Group" src="https://github.com/user-attachments/assets/99a21597-88ca-4d96-bd54-a22c57c65684" />

<img width="1440" height="692" alt="Security Group Owner" src="https://github.com/user-attachments/assets/07ae1361-7ebc-48e0-8664-db444867cba0" />

<img width="1440" height="682" alt="Security Group Users" src="https://github.com/user-attachments/assets/7bec8370-b984-476a-ad32-6cc3a7a8d6c6" />

4. Now that I effectively created both groups and added users to both, I was ready to proceed with the second half of the lab which involved licenses.

### Part 2: Managing Licenses

1. First, I navigated to the 'Group' section from within the Entra admin center. I then selected the 'All groups' option and confirmed that both groups appeared as options. I then selected the security group named 'Sales Admin Group'. When I opened this group's profile, I navigated to the 'Licenses' section and confirmed that no licenses were assigned to this group.

<img width="1439" height="692" alt="Admin Group License pt1" src="https://github.com/user-attachments/assets/74a833f6-5f82-4c67-8729-f77b8ca01707" />

2. Because I have no licenses assigned to the group, I had to utilize the [Microsoft 365 admin center](http://admin.microsoft.com) to assign a license to this group. While within the admin center, licenses are accessed through the menu option labeled 'Billing' and then 'Licenses'.

<img width="1438" height="698" alt="365 Admin Center" src="https://github.com/user-attachments/assets/c962fff8-527b-4865-9fd0-05571ba2597e" />

<img width="1439" height="696" alt="Admin Center Billing" src="https://github.com/user-attachments/assets/6b0a3828-e28c-4f46-ac91-105d63e105bb" />

3. After I identified the licenses that were available, I selected the license I would be applying to the group. * Note, in the README of this repository, I expressed that I acquired a P2 license to utilize the Privileged Identity Management features for future labs*.

<img width="1440" height="700" alt="Available Licenses" src="https://github.com/user-attachments/assets/c1164cfe-d499-4392-b703-530aeea16b81" />

4. While in the P2 license profile, there were two options that displayed who was assigned this license. There was a section for 'Users' and also 'Groups'. I selected 'Groups' and then selected the option to 'Assign licenses'.

<img width="1436" height="692" alt="License Properties " src="https://github.com/user-attachments/assets/f4401477-e71f-40a3-85d7-0bb35375c9c5" />

<img width="1438" height="695" alt="Adding Licenses pt1" src="https://github.com/user-attachments/assets/ecba3633-6e30-4aed-8530-be1eb74204a6" />

<img width="1440" height="695" alt="Adding Licenses pt2" src="https://github.com/user-attachments/assets/26a59201-3959-4442-ac01-0dc0017fff3d" />

5. The licenses were assigned through the 365 admin center but I wanted to confirm that it was properly assigned and applied in Entra. I returned to the Entra admin center and navigated back to the 'Sales Admin Group'. I then  verified under the 'Licenses' options within the group profile that the license was indeed there. This license can be removed from the group entirely through the 365 admin center without affecting any of the individual user's license assignments since the license does not conflict with preexisting licenses and is also not contingent on an add-on. 

<img width="1440" height="676" alt="License Confirmation" src="https://github.com/user-attachments/assets/9b9c0aa1-f05e-458c-ab62-7f4343914408" />

### Security Rationale 

Certain actions or access within Entra is only granted if the necessary licenses are assigned. I had to confirm that the proper licenses were assigned to the group properly. If licenses are not properly assigned including the correct number of licenses correlated to the number of users within the group, then potentially groups with a particular role may not be able to function properly or have correct access. 

### Lessons Learned 

I learned how to assign licenses to groups accordingly. The Microsoft 365 admin center is where group licensing is controlled. This lab provided me with that information and also, confirmed that the Entra P1 and P2 licenses are required for group licensing. 
