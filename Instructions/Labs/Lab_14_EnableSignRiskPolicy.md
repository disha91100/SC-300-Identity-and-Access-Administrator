# Lab 14 - Enable sign in and user risk policies

## Lab scenario

As an additional layer of security, you need to enable and configure your Azure AD organization's sign in and user risk policies.

## Lab Objectives

After completing this lab, you will be able to:
- Task 1 - Configure the policy
- Task 2 - Enable Sign-in risk policy

## Architecture Diagram

![Screen image displaying the New Group page with Group type, Group name, Owners, and Members highlighted](./media/arch14.png)

## Estimated time: 10 minutes

### Before the Hands-on lab

1. Sign in to the [https://portal.azure.com]( https://portal.azure.com) using a Global administrator account.

2. Open the portal menu and then search for and select **Microsoft Entra ID**.

3. On the **Microsoft Entra ID** page, in the left navigation under **Manage**, select **Users**.

4. Select <inject key="AzureAdUserEmail"></inject> 

5. From the **Users** page, in the left navigation under **Manage** select **Assigned Roles**.

   ![Screen image displaying the User risk policy page and highlighted browsing path](./media/assigned-roles.png)

6. Select **+ Add Assignments**. From the list of roles, choose **Conditional Access Administrator** and click on **Add**.
 
   ![Screen image displaying the User risk policy page and highlighted browsing path](./media/assign2.png)

### Exercise 1 - Enable User risk policy

In this exercise, you'll configure a user risk policy in Microsoft Entra ID to block access for high-risk users and enforce password changes. You'll also enable a sign-in risk policy to require multi-factor authentication for risky sign-ins.

### Task 1 - Configure the policy

1. Sign in to the [https://entra.microsoft.com](https://entra.microsoft.com) using a Global administrator account.

2. Open the portal menu and then search for and select **Microsoft Entra ID**.

3. In the left navigation menu, under **Identity**, Select **Protection**.

4. In the left navigation, under **Protection** select **Identity protection**.

    ![Screen image displaying the User risk policy page and highlighted browsing path](./media/image.png)

5. In the Identity protection, in the left navigation, select **User risk policy**.

    ![Screen image displaying the User risk policy page and highlighted browsing path](./media/Screenshot_leftNav.png)

6. Under **Assignments**, select **All users** and review the available options.

7. You can select from **All users** or **Select individuals and groups** if limiting your rollout.

8. Additionally, you can choose to exclude users from the policy.

9. Under **User risk**, select **Low and above**.

10. In the User risk pane, select **High** and then select **Done**.

11. Under **Controls** > **Access**, select **Block access**.

12. In the Access pane, review the available options.

    **Tip** - Microsoft's recommendation is to Allow access and Require password change.

13. Select the **Require password change** check box and then select **Done**.

14. Under **Policy enforcement**, toggle to  **Enabled** and then select **Save**.

### Task 2 - Enable Sign-in risk policy

1. On the Identity protection page, in the left navigation, select **Sign-in risk policy**.

2. As with the User risk policy, the Sign-in risk policy can be assigned to users and groups and allows you to exclude users from the policy.

3. Under **Sign-in risk**, select **Low and above**.

4. In the Sign-in risk pane, select **High** and then select **Done**.

5. Under **Controls** > **Access**, select **Block access**.

6. Select the **Require multi-factor authentication** check box and then select **Done**.

7. Under **Policy enforcement**,  toggle to  **Enabled** and then select **Save**.

## Review

In this lab you have completed the following tasks:

- Configured the policy
- Enabled Sign-in risk policy

## You have successfully completed the lab
