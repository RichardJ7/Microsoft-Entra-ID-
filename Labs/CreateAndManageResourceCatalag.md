# Create and Manage a Resource Catalog 

## Summary 

This lab displays the creation and management of a catalog within Entra. Catalogs contain resources and access packages that can be distributed to different members in a production environment, which is important while overseeing entitlement management. 

### Implementation Steps

Before beginning this lab, it is important to note that entitlement management requires either a Microsoft Entra ID P2 license or Microsoft Entra ID Governance license. I have already acquired a P2 license to provide me with greater capabilities within this learning environment. 

#### Part 1: Creating a Catalog 

1. First, I navigated to the ID Governance menu navigated to the 'Entitlement management' option. Then, I selected the option 'Catalog'.

<img width="1440" height="684" alt="Create a Catalog pt1" src="https://github.com/user-attachments/assets/81ee4bd7-0e3b-4f8c-9b06-f903b2c1d899" />

2. Next, I selected the option 'New Catalog' and began inputting the details necessary for the catalog.

<img width="1440" height="705" alt="Create a catalog pt2" src="https://github.com/user-attachments/assets/4830f26c-aca7-4e33-9985-6572bdace8bb" />

3. In the 'New catalog' pane I completed the 'Name' and 'Description' fields. I then selected 'Yes' for 'Enabled for users to request' and the option 'No' for 'Enabled for external users to request'.

<img width="1440" height="707" alt="Creating a catalog pt3  " src="https://github.com/user-attachments/assets/893678f1-6169-45d3-8b58-dd166eb10b05" />

4. Finally, I selected the option 'Create'.

#### Part 2: Adding Resources

1. From the ID Governance dashboard, I returned to the 'Entitlement Management' pane and selected the 'Catalogs' option to access the newly created catalog.
2. I selected the catalog and then selected the 'Resources' option. After selecting 'Resources', I then selected 'Add Resources'.

<img width="1440" height="706" alt="Add Resources to catalog pt1" src="https://github.com/user-attachments/assets/1814afde-b5b3-411a-a1bc-372eea68df0b" />

3. From this next pane, I selected the different resources to add to this catalog.

<img width="1439" height="705" alt="Adding resources to catalog pt2" src="https://github.com/user-attachments/assets/7d56c4d6-70b3-44f6-bfb1-69d0fb3a3a48" />

4. To complete the addition of these resources to the catalog, select 'Add'. It is important to understand that for these resources to be added to the catalog, they must exist prior to being added and thus, only available resources can be added to the catalog upon its creation. 

### Security Rationale 

In some potential environments, members within the organization and external members can be required to work on a particular project. To prevent these groups from accessing resources beyond the scope of the particular project, catalogs can be implemented, which contain the resources necessary for the completion of the project. By creating a catalog, the specific resources can be actively managed and distributed accordingly, preventing the potential for users to exceed their own access privileges by restricting their access to only necessary resources within the catalog.

### Lessons Learned

Through the completion of this lab, I learned how to create a catalog and manage catalog resources. Being the creator of the catalog, I learned that this also designates the creator as the owner of the catalog. I gained exposure on how to add resources to a catalog and also the navigating the menu options for catalogs. 
