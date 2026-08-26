# Creating Access Reviews 

## Summary 

This lab demonstrates the process of creating access reviews scoped to a particular group in a tenant. Regular reviewing the permissions and access of users in a production environment is typically best practice. This helps with identifying excessive or unnecessary access rights.  

### Implementation Steps

It is important to note that access reviews are only available with at least the Microsoft Entra ID Governance or the Microsoft Entra Suite licenses. 

1. First, navigate to 'ID Governance' blade on the left menu of the dashboard. Then, select 'Access Reviews'.

<img width="1437" height="709" alt="Creating Access Reviews pt1" src="https://github.com/user-attachments/assets/e1b11096-1daf-470d-9bc8-cbffa63447a6" />

2. Next, select the option labeled 'New access review'.

<img width="1437" height="705" alt="Create Access Review pt2" src="https://github.com/user-attachments/assets/e7990971-dadd-4224-920f-224ffa167874" />

3. Two options appear, one labeled 'Review access to a resource type' and another labeled, 'Review users access across multiple resource types within a catalog'. Select the former as this access review will be for resources not for a catalog.

<img width="1439" height="709" alt="Creating Access Reviews pt3" src="https://github.com/user-attachments/assets/d95e6dd3-8e1c-41e8-84f1-ddb6f3321b0a" />

4. Next, input the selections for what is targeted for the review. In this particular access review, the intended target is a particular group.

5. Select the option 'Select Teams + group' and then select the group scope that is the subject of the review.

6. Next, input the scope of the review, including either 'all users' or 'guest users only'.

7. Select the review stages, the reviewers and the recurrence of the review.

<img width="1440" height="705" alt="Creating Access Reviews pt4  " src="https://github.com/user-attachments/assets/cb72fea2-78f6-4615-ab60-76be75f9e505" />

8. Next, input the advanced settings of the review.

<img width="1440" height="709" alt="Creating Access Reviews pt6  " src="https://github.com/user-attachments/assets/70e0c3e5-db02-4d9c-89b0-24fbb8238615" />

9. Finally, select 'Review + create' and name the review.

### Security Rationale

Access reviews are essential in production environments. Users can be given permissions or access to resources for a particular project and once the project is completed, they still have those permissions. This is a security risk because users now have permissions that exceed their daily role. Stale permissions can jeopardize a production environment, thus one of the most effective practices in preventing the security issues related to stale permissions


