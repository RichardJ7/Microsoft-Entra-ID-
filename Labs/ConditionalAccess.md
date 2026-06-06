# Conditional Access

## Summary 

The purpose of this lab is to learn how to implement Conditional Access wihtin Microsoft Entra. Conditional Access can be reduced to if-then statements that are implemented into an organization to control access and enforce a Zero Trust environment. Conditional Access is provides great flexibility in terms of the conditions that can be altered in order to achieve the overall goal of a secure posture. In this lab, I explored the different conditions in addition to how to properly create a policy to achieve an intended goal.  

### Implementation Steps

To preface this lab, a few key points should be noted. First, Conditional Access requires at least a Microsoft Entra ID P1 license at minimum. Policies that are risk-based require a Microsoft Entra ID P2 license. Second, Conditional Access cannot be enabled while security defaults are actively enabled. Security defaults must first be disabled before Conditional Access policies can be constructed. I have already purchased the necessary licenses for the labs related to Entra so I will not be documenting those steps below. I will begin by documenting security defaults. 

#### Part 1: Disabling Security Defaults

1. First, log-in to the Microsoft Entra Admin center and navigate to the 'Overview' section underneath the Entra ID menu. 

<img width="1434" height="708" alt="Disabling Security Defaults pt1" src="https://github.com/user-attachments/assets/c4cc6548-941b-4768-99ce-5612ba9f64eb" />

2. After selecting 'Overview', select the 'Properties' tab and scroll to the bottom. The 'Security Defaults' setting should be available.

<img width="1440" height="687" alt="Disabling Security Defaults pt2" src="https://github.com/user-attachments/assets/76579e59-be3a-42e6-bc13-daa4093a3b8f" />

3. Select the option 'Manage security defaults' and then select in the drop down menu that appears to the right 'Disabled'. Then select 'My organization is planning to use Conditional Access' as the reason for disabling. Then, select 'Save' to apply the setting.

<img width="1440" height="710" alt="Disabling Security Defaults pt3  " src="https://github.com/user-attachments/assets/36e58372-ab4a-4fc8-965a-03e4ccfbe6c3" />

#### Part 2: Creating Conditional Access Policies

1. Now that security defaults are disabled, navigate to 'Conditional Access' under the Entra menu blade.

<img width="1437" height="687" alt="CA Policy pt1  " src="https://github.com/user-attachments/assets/1c671264-8ece-42a5-92d2-9c05a2db8efb" />

2. While in the main menu for Conditional Access, select 'Create New Policy'.
3. The creation of the policy begins with first naming the policy.
4. After naming the policy, you must first configure the 'Assignments', which is who the intended policy is supposed to affect.
5. Once the assignments are designated, the next selection is 'Target Resources'. These are the resources that the assignments access that trigger the policy to be evaluated.
6. After, the 'Conditions' must be configured. The 'Conditions' section allows for granular control over what conditions must be met for a user to be either granted or blocked access in the intended policy.
7. Once the 'Conditions' are selected, the 'Access Controls' must be selected with the option as mentioned being either 'Grant' or 'Block' access.
8. Finally. the policy must be enabled. Under 'Enable Policy' select 'On'. Note that in actual environments the policies created should first be enabled in Report-only mode to view the implementation of the policies within the environment. Report-only mode allows administrators to view the policy's impact in the environment first through monitoring the sign-in logs and how it affects users. Once the policies impact is evaluated it should be set to 'On'. For Microsoft enabled Conditional Access policies, those set in Report-only mode will be automatically enabled and set to On in 45 days if left in Report-only mode. 

You can view the Conditional Access policy creation here! [Conditional Access Tutorial](https://vimeo.com/1156325629/b784f45505?fl=ip&fe=ec)
