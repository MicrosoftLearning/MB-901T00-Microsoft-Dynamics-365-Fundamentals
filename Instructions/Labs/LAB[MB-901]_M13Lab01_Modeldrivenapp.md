---
lab:
    title: 'Lab 01: Build your first model-driven app from scratch'
    module: 'Module 13: Connect and analyze your Dynamics 365 data'
---

# MB-901: Dynamics 365 Fundamentals
## Module 14, Lab 1: Build your first model-driven app from scratch

**Scenario:** You need to simplify create a model-driven app by using one of the standard entities that's available in your Power Apps environment. Model-driven apps don't run in the Power Apps mobile app. Instead, you run a model-driven app on a mobile device using either the Dynamics 365 mobile app or in the phone's web browser.

Sign in with your window’s live id to Power Apps. If you don’t already have a Power Apps account, select the Get started free link from https://signup.microsoft.com/Start?sku=powerapps_viral&ru=https%3a%2f%2fweb.powerapps.com%2flogin%2fportal

## Instructions
1. Access the Power Platform Admin Center.
12.	Select **Environments**.
13.	Select your trial CRM environment. 
14.	Select ![Dynamics 365 Administration Center](https://port.crm.dynamics.com/G/Instances/InstancePicker.aspx?redirect=False0) hyperlink.
15.	Select **GTLPowerApps**.
16.	Select **Open**.
17.	Select **Create new App**.
19.	On the **Create a New App** page, enter the following details, and then select **Done**:
    - **Name:** Type **GuideToPowerApp**.
    - **Unique Name:** By default, the unique name uses the name you specify in the Name box without spaces and preceded by the publisher prefix and an underscore (_).
    - **Description:** Type **GuideToPowerApp**.
20.	Select **Done**.
21.	From the app designer you add components to your app. Select pencil icon on the **Site Map** button to open the sitemap designer.
22.	You are going to use Accounts entity in this power app to manage customer accounts.
22. On the **Properties** tab, type **Accounts** for the Area name.
23.	On the sitemap designer select **New Subarea**, in the right pane select the **Properties** tab, and then select the value of following properties:
    - **Type: Entity**
    - **Entity: Account**  
    - Select **Save.** 
24.	Select **App Designer**.
25.	On the app designer canvas select **Forms**, and then on the right pane under the **Main Forms** group select the **Account** form.
26.	Select the **back** button.
27.	On the app designer canvas select **Views**, and then select the **Active Accounts**, **All Accounts**, and **My Active Accounts** views.
28.	Select the **back** button.
29.	On the app designer canvas select **Charts**, and then select the **Accounts by Industry chart**.
30.	Select the **back** button.
31.	On the app designer toolbar, click **Save** and then **Publish**.
32.	Select **Play**.
34.	Review the results and interact with your first model-driven application.
35.	Try it on your mobile device by Installing the Dynamics 365 for phones or Dynamics 365 for tablets app from your device’s app store. More information: https://docs.microsoft.com/dynamics365/customer-engagement/mobile-app/install-dynamics-365-for-phones-and-tablets
36.	Enter the application URL directly into your phone’s web browser and follow the directions on your screen to load the app. 
  **Note:** An example of your application URL will look like the following: https://orgxxxxx.crm.dynamics.com/main.aspx?appid=e4547538-e20f-ea01-a811-000d3a33438d&pagetype=entitylist&etn=account
