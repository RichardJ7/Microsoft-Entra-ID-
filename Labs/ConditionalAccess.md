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
