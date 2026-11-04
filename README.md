# Modern-Workplace-Onboarding-Microsoft-Entra-ID-Intune-M365
Onboarding solution using Microsoft Entra ID, Intune, and Microsoft 365 to automate user provisioning, identity management, device enrollment, and access configuration.

## QUICK DEFINITIONS
1) **Microsoft Entra ID**:
A cloud-based IAM (Identity and access management) service. It manages Identities and helps control access to other tools. Entra ID is particularly good for User identity **(employees, contractors, guests)**, **Authentication(Password, MFA, SSO)**, **Access control(groups, policies)**

2) **Microsoft Intune**:
It manages company laptops, desktops, phones, apps, and security settings.

3) **Microsoft 365**:
It is a cloud PC service. It gives an employee a personal Windows desktop hosted in the cloud, and the employee can access tools like Teams, Outlook, etc

## PREREQUISITS

1) **Two virtual machines**: One will be used for Admin, and the other will be the Agent.
   ![Onboarding](./Images/P0.JPG)
3) **Download and install two Windows 11 Enterprise** from the Microsoft official website (you will have to create an account. Iso is valid for 90 days)
4) **Obtain Microsoft Entra ID, Intune, and M365**:There are different ways to have these tools, and you are free to purchase or download a trial version. I purchased trial versions of Intune and M365. It gave me access to Entra ID.

## ONBOARDING
Onboarding happens when someone is hired. The HR and IT teams coordinate to make onboarding successful.

**Example**: You receive a ticket from the HR département to onboard a new employee in the company. 
As an IT Support agent, you have to:

-	Create the employee’s Identity (Entra ID)
-	Assign access and licenses (EntraID-M365)
-	Prepare their device (INTUNE)
-	Configure security ( INTUNE)
-	Verify everything works

 1)	**Create the employee’s identity**
Let's create an Agent called **Hanna Montana**

![Onboarding](./Images/C12.JPG) 
![Onboarding](./Images/C2.JPG)
![Onboarding](./Images/C4.JPG)

This information can be filled in later when the account has been created. Right now, I will just give it a first name, last name, and Job title.


![Onboarding](./Images/C6.JPG)

Once you are done, you will receive a confirmation message and refresh the page to see you employee.


![Onboarding](./Images/C7.JPG)


2) **Assign access and licenses (EntraID or M365)**

Right now, Miss Montana has no licenses and can't access Teams or Outlook
![Onboarding](./Images/A1.JPG)

We will use M365 for this step

![Onboarding](./Images/A2.JPG)


![Onboarding](./Images/A4.JPG)

3) **Prepare and enroll device in Intune**
**NB**: For this to work, you must  have Windows 10 or 11 Enterprise version: **Cloud enrollment and Company Portal**
There are two ways of doing this. We will start with **Cloud enrollment**.

-Go to Settings → Accounts → Access work or school.
-Click Connect.
-Select Join this device to Microsoft Entra ID.
-A password reset may be requested. Follow the on-screen instructions and complete the process.
-Once completed, the system will update and synchronize.

You can now access Microsoft Entra ID, Intune, Microsoft 365, and Azure without repeatedly entering your password.
![Onboarding](./Images/P1.JPG)
![Onboarding](./Images/P2.JPG)
![Onboarding](./Images/P3.JPG)
![Onboarding](./Images/P4.JPG)
![Onboarding](./Images/P5.JPG)
![Onboarding](./Images/P6.JPG)
![Onboarding](./Images/P7.JPG)

Now, your device has been joined, and you can see it in Entra ID, but it is not visible in Intune
![Onboarding](./Images/P10.JPG)
![Onboarding](./Images/P11.JPG)



##### To enroll your PC and give your company full administrative rights, you need to download and install the **Company Portal**


![Onboarding](./Images/P12.JPG)
![Onboarding](./Images/P13.JPG)
![Onboarding](./Images/P14.JPG)
![Onboarding](./Images/P15.JPG)
![Onboarding](./Images/P16.JPG)

The computer is all set.
There are a few more steps that have to be done
-	Configure security and compliance (Intune)
-	Microsoft Services (M365)
-	Configure any required Azure resources (AZURE)
-	Test the employee sign-in and access
-	Hand over the equipment and close the ticket


## CONCLUSION
This project demonstrates the employee onboarding process using Microsoft Entra ID, Microsoft Intune, and Microsoft 365. By joining devices to Entra ID and enrolling them through Company Portal, users can securely access organizational resources while enabling centralized identity and device management.
