---
lab:
    title: 'Explore Microsoft Entra ID User Settings'
    module: 'Describe the function and identity types of Microsoft Entra ID'
---

# Lab: Explore Microsoft Entra ID User Settings

This lab maps to the following Learn content:

- Learning Path: Describe the capabilities of Microsoft Entra.
- Module: Describe the function and identity types of Microsoft Entra ID.
- Unit: Describe the types of identities.

## Lab scenario

In this lab, you'll access Microsoft Entra ID (previously referred to as Azure Active Directory).  Additionally, you'll create a user and configure the different settings, including adding licenses.  

**Estimated Time**: 30 minutes

### Task 1

As a subscriber to Microsoft 365 you're already using Microsoft Entra ID.  In this task, you’ll learn how to create a new user in Microsoft Entra ID and explore some of services that can be managed at the user level.

1. Open the Microsoft Edge browser. In the address bar, enter **`https://admin.microsoft.com`** and sign in with the Microsoft 365 credentials provided by your authorized lab hoster (ALH).
    1. In the Sign-in window, enter **admin@WWLxZZZZZZ.onmicrosoft.com** (where ZZZZZZ is your unique tenant ID provided by your ALH) then select **Next**.
    1. Enter the admin password that should be provided by your lab hosting provider. Select **Sign in**.
    1. Depending on your lab hoster and if this is the first time you are logging in to the tenant, you may be prompted to complete the MFA registration process. If so, follow the prompts on the screen to setup MFA.
    1. Once you're signed-in, you're taken to the Microsoft 365 admin center page.

1. Under Admin centers, select **Identity** (you may need to select **Show all** and scroll down).  A new browser page opens to the overview page of the Microsoft Entra admin center.

1. From the left navigation pane, expand **Users** then select **All users**. Notice that your tenant is already configured with users.

1. From the top of the page, select **+ New user** then from the drop-down box, select **Create new user**.

1. You are now in the **basics** tab of the create new user page. Populate the fields as follows:
    1. User principal name: **sara**.

    1. Mail nickname: leave the default, which is set to derive from user principal name.

    1. Display name: **Sara Perez**.

    1. Password: uncheck the box that says auto-generate password and enter a temporary password that adheres to the password requirements and make note of it, as you will need it to complete the subsequent task.

    1. Account enabled:  Leave the checkmark to ensure the account is enabled.

    1. At the bottom of the page, select **Next: Properties**.

1. Here you will configure a few of the fields in the **Properties** tab.

    1. First name: Sara

    1. Last name: Perez

    1. User types:  Leave the default to **Member**, but note that from the drop-down you have the option to select guest.

    1. Usage location: Choose the country/region where you are located.  Note that to get to the usage location field, you will need to scroll down on the page as it is the last field on the page.  **NOTE**: if you don't do this, you will not be able assign a license in a subsequent step.

    1. Select **Next: Assignments**.

1. You are now on the **Assignments** tab where you add a group assignment and view the available options for adding a role.

    1. Select **Add group**.

    1. The window that opens shows all the available groups.  

    1. Notice the list of available groups.  From the list, select **Operations**.  From the bottom of the page, select the **Select** button.  It may take a few seconds but you should see the operations group showup on the assignments page.

    1. From the top of the page, select **+ Add role**.  A window opens that shows all the available directory roles.  View the available options, but don't add any new roles.  Close this page by selecting the **X** on the top right corner of the directory roles page.
    1. From the bottom of the page, select **Review + create**. A summary of the settings will be displayed.  From the bottom of the page, select **Create**.

1. You are returned to the users page.  After a few seconds, Sara Perez will be listed.  You may need to select the **refresh** icon on the top of the page.

1. From the user list, select the user you created, **Sara Perez**.  The **Overview** page opens.

1. The left navigation panel shows the various options that can be configured for the user. View the available options.

1. From the left navigation panel, select **Licenses**.  Notice that there are no license assignments found for this user, also note the warning icon that says, "Adding, removing, and reprocessing licensing assignments is only available within the M365 Admin Center."  You'll do that in the next task.  NOTE:  Licenses can only be assigned if a usage location was configured. If you did not set the usage location, go back to that step now.

### Task 2

In this task, you’ll assign a license to the user you just created, using the Microsoft 365 admin center.

1. Open the browser tab **Home - Microsoft 365 admin center**.

1. From the left navigation panel, under users, select **Active users**.  From the list of users, select **Sara Perez**.  A window opens showing information about the user.  

    1. Select the **Licenses and apps** tab.
    1. For each of the licenses listed, you see number of available licenses.  Since there are no available Microsoft 365 E5 licenses (they have already been assigned to other users), assign the **Microsoft Power Apps Developer** and the **Microsoft Power Automate Free** licenses by selecting the check box next to them.
    1. Select **Save changes**. A notification on the top right corner of the screen should show that license assignments succeeded.
    1. Close the page by selecting the **X** at the top right corner of the page.

1. Return to the Microsoft Entra admin center by selecting **Home** from the left navigation panel or from the top-left of the screen (the bread-crumb), above where it says Sara Perez | Licenses.

1. You have successfully assigned licenses to the user.

1. Sign out of all the open browser tabs. Sign out by selecting the user icon next to the email address on the top right corner of the screen then selecting **Sign out**. Close all the browser windows.

### Task 3

In this task, you'll sign in as Sara Perez, for the first time.

1. Open Microsoft Edge.

1. In the address bar, enter **https://login.microsoft.com**.

1. Sign in as **sara@WWLxZZZZZ.onmicrosoft.com**, (where ZZZZZZ is your unique tenant ID provided by your ALH)
1. Enter the temporary password you set in the previous task.

1. You are now prompted to Update your password. In the Current password field, enter the temporary password from the previous task.

1. In the New password field, enter a new password, confirm the password, then select **Sign in**.  Make note of your new password as you will need it for the subsequent lab exercise on SSPR.

1. Since this is the first time you are logging in as Sara Perez, you may be prompted to setup MFA. Follow the prompts on the screen to setup MFA.

1. You should now be successfully signed-in to Sara's Microsoft account.  Note that Sara's licensing that you assigned in the previous task was limited only to Power Automate Free and Power Apps for Developer and did not include E5 licensing.

1. Sign out by selecting the icon on the top right corner of the Microsoft 365 window that is shown as a circle with the letters SP (next to the question mark icon), then selecting **Sign out**, then close the browser.

### Review

In this lab, you started your initial exploration of Microsoft Entra ID. Since subscribers to Microsoft 365 are automatically using Microsoft Entra ID, you found that you access Microsoft Entra ID features and services through either the Microsoft 365 admin portal or through the Azure portal.  Whichever approach you prefer to get to the same place.  You also walked through the process of creating a new user and the different setting that can be configured, including groups to which the user can be assigned, the availability of roles, and assigning of user licenses.
