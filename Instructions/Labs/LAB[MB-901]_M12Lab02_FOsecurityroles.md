---
lab:
    title: 'Lab 02: Explore security roles in Dynamics 365 Finance and Operations applications'
    module: 'Module 12: Recognize Dynamics 365 security'
---

# MB-901: Dynamics 365 Fundamentals
## Module 12, Lab 2 - Explore security roles in Dynamics 365 Finance and Operations applications

### Exclude role

**Scenario:** The HR department of USMF has requested to remove access to the Accounts receivable clerk role in Dynamics 365 Finance and Operations applications for an employee who has changed role. You, as a system administrator need to exclude Accounts receivable clerk role for the employee.

1. Go to **System administration** > **Security** > **Assign users to roles**.
1. In the tree, select **'Accounts receivable clerk'**.
1. Select **Manually assign** / **exclude users**.
1. In the list, select a user.
1. Select **Exclude from role** to exclude the selected users from the role.
1. To remove exclusions, select the users that you want to remove exclusions for, and then click **Reset status**. 

### Create segregation of duties rule

**Scenario:** The HR department of USMF has requested having a rule for segregation of duties for **Access benefits workspace** as the first and **Approve production journal** as the second duty. You, as a system administrator need to create the rule.

1. Go to **System administration** > **Security** > **Segregation of duties** > **Segregation of duties rules**.
1. Select **New**.
1. In the **Name** field, enter a name for the rule.
1. In the **First duty** field, click the drop-down button to open the lookup.
1. In the list, find and select the first duty that is controlled by the rule.
1. In the list, click the link in the selected row.
1. In the **Second duty** field, click the drop-down button to open the lookup.
1. In the list, find and select the second duty that is controlled by the rule.
1. In the list, click the link in the selected row.
1. In the **Severity** field, select the severity of the risk that occurs when the same user or role performs both duties.
1. In the **Security risk** field, enter a description of the security risk.
1. In the **Security mitigation** field, type a value.
1. Enter a description of the actions that you take to mitigate the security risk. 
For example, you can mitigate the risk by conducting more detailed reviews of the process, by conducting a monthly managerial review, or by sharing resources with other departments.
1. Select **Save**.
