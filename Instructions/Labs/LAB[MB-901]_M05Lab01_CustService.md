---
lab:
    title: 'Lab 01: Explore Dynamics 365 Customer Service'
    module: 'Module 05: Introduction to Dynamics 365 Customer Service '
---

# MB-901: Dynamics 365 Fundamentals 
## Module 5, Lab 1 - Explore Dynamics 365 Customer Service 

**Scenario:**
As a customer service representative, you need to keep track of your customer requests and issues by creating support cases in Dynamics 365 Customer Service. When a customer contacts support with a question or problem, you can quickly check if there is an existing case or open a new case and start tracking the issue. You can also escalate, reassign, or put a case back into the service queue if you don’t have enough information or time to work on it.

Before you provide support, you can also check the customer’s entitlements. Entitlements are like contracts that tell you what kind of support a customer is eligible for. You can see if the support terms are based on number of hours or cases, support channel, or based on the product or service that the customer has purchased.

To help you select the right status of a case, your administrator may have set things up so that you only see a limited set of statuses based on the current status of a case.

## Instructions

### Create a case

1. In the **Customer Service Hub**, go to **Service** > **Cases**.
1. Select **New Case**.
1. In the **Case Title** field, type **Seahorse Smart Watch**.
1. In the **Customer** field, select customer **Fabrikam** and select an existing record for the account.
1. In the **Description** field, type **Issue with the Smart watch**
1. Click **Details** tab.
1. Click **Save**.
1. To track your conversation with the customer, in the **Timeline** section click **+** to add info and activities.
1. Click **Note**.
1. In the **Title** field, type **Smart Watch Defect**.
1. In the **Note** field, type **Send for repair**.
1. Click **Add note**. 
14.	To see what kind of support you should provide the customer, select the **Entitlements lookup** button and select an active entitlement.
 **Note:** If there is no entitlement on the customer, this will be blank.
1. Click **Save**.

### Find a solution from similar cases

**Note:** You can look at resolved cases to see if they can help you resolve the open case you’re working on. For example, if the subject of the case you’re working on is “**Smart Watch Defect**” you could look for resolved cases with the same subject to get help with your current case.

### Resolve a case

Before you resolve a case, make sure that all the case activities are closed. Otherwise, you’ll get a message saying that you still have open activities associated with the case, which will be canceled if the case is resolved.

1. Go to **Service** > **Cases**.
1. In the list of active cases, open the **Seahorse Smart Watch** case to resolve.
1. On the command bar, select **Resolve case**.
1. In the **Resolve Case** dialog box, in the **Resolution Type** list, select **Problem Solved**.
1. In the **Resolution** box, type **Repaired**.
1. The actual time spent on all activities for this case, as recorded in the **Duration** box in each activity, is filled out automatically in the **Total Time** box.
1. In the **Billable Time** list, select **30 minutes** as the amount of time spent on the case to be billed to the customer.
 **Note:** If this case is linked to a contract or entitlement, the billable time will be subtracted from the allotted minutes for that contract.
1. Select **Resolve**. A case resolution activity is created and shown in the **Activities** area. 

The resolution activity contains information about a resolved case, including the resolution and total time spent on the case. You can reactivate a resolved case at any time.
