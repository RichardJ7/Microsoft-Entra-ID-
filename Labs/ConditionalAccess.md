# Conditional Access

## Summary 

The purpose of this lab is to learn how to implement Conditional Access wihtin Microsoft Entra. Conditional Access can be reduced to if-then statements that are implemented into an organization to control access and enforce a Zero Trust environment. Conditional Access is provides great flexibility in terms of the conditions that can be altered in order to achieve the overall goal of a secure posture. In this lab, I explored the different conditions in addition to how to properly create a policy to achieve an intended goal.  

### Implementation Steps

To preface this lab, a few key points should be noted. First, Conditional Access requires at least a Microsoft Entra ID P1 license at minimum. Policies that are risk-based require a Microsoft Entra ID P2 license. Second, Conditional Access cannot be enabled while security defaults are actively enabled. Security defaults must first be disabled before Conditional Access policies can be constructed. I have already purchased the necessary licenses for the labs related to Entra so I will not be documenting those steps below. I will begin by documenting security defaults. 

1. 
