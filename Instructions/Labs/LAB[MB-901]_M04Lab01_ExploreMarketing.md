---
lab:
    title: 'Lab 01: Explore Dynamics 365 Marketing'
    module: 'Module 04: Introduction to Dynamics 365 Marketing'
---

# MB-901: Dynamics 365 Fundamentals 
## Module 4, Lab 1 -Explore Dynamics 365 Marketing

**Prerequisites:** Prior to performing the steps of this lab, perform the following tasks: 
1. Go to **Marketing** > **Files**.
1. Click **New**.
1. Click **Add files**.
1. Upload at least one image from your desktop.
1. Click **Upload**.
1. Once the upload is complete, click **Done.**

### Create engaging emails

1. Go to **Marketing** > **Marketing Emails**. This takes you to a list of existing marketing emails. Select **New** on the command bar.
1. The **Marketing email templates** dialog box opens. For this exercise, select **Skip**, so that you can start with a blank template and step through all the required content. **Tip:** Several standard templates are provided out of the box, and you can also create your own templates that feature your organization's graphical identity, required elements, and messaging standards. More information: https://docs.microsoft.com/dynamics365/marketing/create-templates) 
You now have the **New Marketing email** page open.
1. From the dropdown next to the **Name** and **Status reason** fields in the upper right corner, select the down arrow to open a drop-down dialog and then enter a **Name** for your new message.
1. Enter a **Subject** for your message. This is a very important setting because this is one of the first things recipients will see when they receive the email, and they may use this to decide whether or not to read the message.
1. In the main part of the page, you now see the design canvas (on the left side), where you can drag, arrange, and enter content. Since you chose the blank template, your design includes just a single one-column section (layout) element with nothing in it. 
1. A **Toolbox** on the right side of the page provides design elements that you'll use to construct your message. Drag a **Text** element from the **Toolbox** tab into the section element. When you have dragged the element to a suitable location, a blue shaded region appears. Release the mouse button to drop the element at that location.
1. When you drop the text element, you'll see some placeholder text within the element and a floating toolbar just below or above it.
1. Select and remove the placeholder text, and then add your own. Use the toolbar buttons to style your text as you would in a text editor like Microsoft Word (point to any toolbar button to see what it does). Most of the buttons are for styling text and paragraphs, but there are also buttons for creating links; entering dynamic text (more on this later); and moving, copying, or deleting the entire text element. **Tip:** The very first text that you enter on the page is especially important because most email clients show this as preview text for the messages in their inbox list. Here is how it looks in Microsoft Outlook:
1. An easy way to personalize the message is to include the name of the recipient in the greeting. Add the recipient's name as dynamic text by using the **Assist edit </>** feature as follows:
    - Working in the text element you just added, enter a suitable opening such as "Dear".
    - On the pop-up toolbar, select the Assist edit button. This opens the assist-edit dialog.
    - **Note:** Assist edit helps you construct valid dynamic expressions to position field values from recipient contact records, the message content settings, and other database values. This button is provided on the text formatting toolbar whenever you select a text element in the graphical designer. The button is also provided for some settings fields, such as the subject, from-address, and from-name fields.
  - Select the **Dynamic content** radio button, and then select **Contact** from the combo box here. The **Dynamic** setting means that you will place a dynamic value related to the context where you use the message, while the **Contact** setting means that the context relates to the individual recipient (contact) of the message.
  - Select **No relationship** for relationship.
  - On the previous page, you choose the contact settings entity (in context). On this page you must choose which field from that entity you want to place. We're building the salutation, so we'd like to show the recipient's name here. Select the **Select field** radio button and then start to type "First Name" into the combo box here. This searches the available fields for those that include the text "First Name", which greatly reduces the number of fields you need to look through. Select **First Name** from the list as soon as you can see it. 
  - Select **Insert** to place the expression you've built and close the assist-edit tool. The full salutation now looks like this: **Dear {{contact.firstname}},**.  **Tip:** You might have noticed that the **Subject** field also has an assist-edit button. This means that you can put dynamic text (including the recipient's name) in the subject too.
11.	The body of all email messages must include both a subscription-center link and your organization's physical address. These are required by law in many jurisdictions, and **Dynamics 365 Marketing** won't let you publish any marketing email that doesn't have them. Place them by using assist edit as follows:
  - Choose a suitable location for your **address**, and then use assist edit to place it. Select **Dynamic** and then **Select entity** on the first page of the assist-edit tool. Select **Contact** and then pick **No relationship**. For **Select Field** and **Address 1** on the second page. Select **Insert** to place the expression {{msdyncrm_contentsettings.msdyncrm_addressmain}} into your message.
  - Choose a suitable location for the subscription-center link, and then enter some anchor text there (such as "Manage your subscriptions"). Select the anchor text, and then select the **Link** button from the floating toolbar, which opens the **Link** dialog box. Select the **Assist edit** button for the **Link** field. In the assist-edit dialog, select **Dynamic** and then **ContentSettings** on the first page. Select **No relationship.** For select field select **subscriptioncenter** on the second page. 
  - Select **Insert** to place the expression {{msdyncrm_contentsettings.msdyncrm_subscriptioncenter}} into the **Link** field. Then select **OK.**
12. You should usually include at least one visible image in your design because this will invite recipients to load images, which is required for Dynamics 365 Marketing to log the message-open event. Drag an **Image** element from the **Toolbox** onto the canvas. This time, when you drop the element, you'll see an image placeholder and the **Properties** tab, which shows configuration settings for the selected element.
13. On the **Properties** tab, select the **Image gallery** button  at the right side of the **Source** field. The **Select a file** dialog box opens. Here you can see all the images that have already been uploaded to your Dynamics 365 Marketing server. Select an image, and then choose **Select** to place it in your message design. (If you don't see any images, choose Upload to add a new one.)    
- **Tip:** When a message goes live, **Dynamics 365 Marketing** uploads all relevant images from your library to its content-delivery network, where they become available as a single source to all recipients. The images aren't attached to each message, but instead are included as links that are redirected through **Dynamics 365 Marketing** for tracking purposes. Recipients won't download any images until they open the message, which saves bandwidth both for you and them. When a recipient's email client requests the images, **Dynamics 365 Marketing** knows that the message has been opened, and by whom.
1. Your message now includes all the minimal required and recommended content, so go to the **Preview** tab to see an approximation of how it will be rendered on various screen sizes and how its dynamic content will get resolved. Use the buttons in the leftmost column to choose a screen size and orientation to preview. Use the **Contact** and **Content Settings** fields in the **Properties** column to see how your dynamic content will resolve for various recipients and settings.
1. To make sure your message includes all required content and is ready to send, select **Check for Errors** in the command bar. Dynamics 365 Marketing checks your message, and then displays results in the notification bar at the top of the page. If more than one error is found, then select the expansion button to see all of them. If you followed this procedure, your message should pass the error check. If it doesn't, read the error message, fix the reported issue, and try again until it passes.
1. Until now, your previews and error checks have been simulated. The final test is to deliver the message to yourself, open it in your email program, and inspect the results. On the command bar, select **Test Send**. A **Quick Create** form slides in from the side. Enter your own **Email Address** in the field provided, and select the **Test Contact** and **Test Content Settings** records to use when resolving dynamic content (these work the same as for the simulated preview). Select **Save** to send yourself the message. You should receive it in a few minutes.
1. If your message still looks good after you receive it in your inbox and open it, you're ready to publish it by selecting **Go Live** on the command bar. **Dynamics 365 Marketing** copies your design to the email marketing service, which makes the message available for use by a customer journey (but doesn't deliver any messages yet). The go-live process also activates any dynamic code and replaces links with trackable versions that are redirected through **Dynamics 365 Marketing** (which identifies the recipient and logs the click). Finally, your message **Status Reason** is updated to Live.
  - **Tip:** While the message is live, it's locked for editing in Dynamics 365 Marketing. If you need to edit a live message, you must first open it in Dynamics 365 Marketing, and then select **Deactivate** on the command bar.
  
### Pinpoint your audience

**Scenario:** You need to set up a collection of segments, which you'll define by using terms that resemble those you already use to describe groups of customers. 
Then you'll use these segments to target marketing initiatives like email-marketing campaigns and customer journeys. Segments like these, which you define by using a set of rules and conditions, are called dynamic segments because membership in these segments changes constantly and automatically based on information in your database. Note: Static segments are populated by adding contacts explicitly, one at a time.

1. Go to **Marketing** > **Contacts**. This takes you to a list of existing contacts. On the command bar, select **New**.
1. The **New Contact** page opens. Fill out the following fields:
 - **First Name:** Enter a fictional first name.
 - **Last Name:** Enter a fictional last name.
 - **Email:** Enter your own email address (or one that you can receive mail from).
 - **Address 1: City:** Enter a fictional city (for this example, we use **Atlantis**). This will make it easy to create a segment that only includes fictional contacts. 
1. On the command bar, select **Save & Close**.
1. Create a second contact similar to the one you just made. Use the same email address and fictional city, but use a different first and last name.
1. On the command bar, select **Save & Close**.
1. Go to **Customers** > **Segments**. This takes you to a list of existing segments. On the command bar, select **New Dynamic Segment.**
1. A pop-up screen will appear, where you can select a segment template. Click **Skip**.
1. The **New Segment** page opens.
1. **Dynamics 365 Marketing** creates a demographic segment, which already includes a query against the contact entity. You can see the **Contact** entity being queried by checking the value shown on the drop-down list at the top of the query block. 
1. Your segment currently includes no filters (clause rows), which means it will find all the contacts in your database. But we only want to find the new test contacts that we just created, so let's add a filter.
1. The **Select attribute** field to open a drop-down list that shows all attributes available on the contact entity. Then type "city" to filter the list and choose **Address 1: City** from the list.
1. Two new drop-down lists are now added to the row. Leave the next drop-down list set to **Equals**. This is the operator, which defines the way we are going test values in the **Address 1: City** field of the **Contact** entity. Other operators include **Contains**, **Begins with**, **Contains data**, and more, depending on which type of value (string, number, date, and so on) you are working with.
1. Select the third drop-down list, which contains the ghost text **Enter text** and type the fictional city name that you chose for your test contacts (such as "Atlantis" if that's what you chose).
1. Select the field at the top of the query, which contains the ghost test **Enter segment name** and enter a name for your segment (such as "Contacts from Atlantis").
1. Select **Save** on the command bar to save your segment and then select **Go Live** to publish the segment (you won't be able to use it in a customer journey until it goes live, even though you've saved it). Dynamics 365 Marketing checks the segment for errors and reports any problems it finds. If an error is reported, fix it and try again. If no error is found, your segment is copied to the marketing services, which make it available for use by a customer journey.
1. Wait for about a minute and then select **Refresh** on the command bar to refresh the page. You should now see that a **Members** tab has been added (if you don't see it, wait a little longer and try to **Refresh** again until you do). When the **Members** tab appears, open it and note that your segment includes the two fictional contacts that you added earlier.

### Build a campaign 

**Scenario:** You need to create a customer journey that executes a one-time email blast.

1. Go to **Marketing execution** > **Customer Journeys**. This takes you to a list of existing customer journeys. Select **New** on the command bar.
1. The **New Customer Journey** page opens with the **Select a Customer Journey Template** dialog box shown. Select **Skip**, and then choose **Select**. The dialog box closes, and your selected template is copied to your new journey.
1. Now you are looking at the customer journey designer, where you will assemble a pipeline that defines each step of the journey. Like all journeys, this one starts with the participants, who in this case are the people you specify as part of a market segment. Drag a **Segment** tile from the **Toolbox** tab onto the first position of the pipeline.
1. Select the expand button at the lower-right corner of your new **Segment Group** tile to view the member segments of this group. Right now, there's just one, so select it.
1. With the nested segment still selected, open the **Properties** tab to the right of the canvas. The **Properties** tab provides settings that apply to the selected tile. Set the **Segment** to the name of the segment that you want to target with your campaign.
1. Go back to the **Toolbox** tab and drag an **Marketing email message** tile to the space immediately to the right of the **Segment Group** tile.
1. With the new **Email** tile still selected, open the **Properties** tab again. Set the **Marketing Email Message** to the name of the message that you created earlier in the Create engaging emails section of this lab.  
1. Until now, you've been working on the **Designer** tab. Now go to the **General** tab, where you can name your journey and configure its run schedule. Make the following settings here:
 - **Name:** Enter a name for the customer journey that you can easily recognize later. This name is internal-only.
 - **Start Date and Time:** Enter the time when the journey should begin processing contacts. When you select the field, a suggested default time is provided.
 - **End Date and Time:** Enter the time at which the journey should stop processing contacts. All actions will stop at this time, even if some contacts are still in the middle of the journey. If you're just testing, allow a couple of weeks.
 - **Time Zone:** Select your local time zone (if needed). The other dates and times on the page will be displayed relative to this zone. 
 - **Content Settings:** This should already be set to the default content settings record set for your instance. 
1. On the command bar, select **Save** to save the work you've done so far.
1. To make sure your journey includes all required content and settings, select **Check for Errors** in the command bar. **Dynamics 365 Marketing** checks it and then displays results. If errors were found, you'll see a message at the top of the window and various indicators to show where the problems are. For example, if one of your tiles is misconfigured, you'll see an error count above the relevant tile, and you can read details about the error by selecting the tile and opening its Properties tab.
1. If you followed this procedure and your email message is live, your journey should pass the error check. If it doesn't, read the error message, fix the reported issue, and try again until it passes.
1. Your journey is now ready to go. To start it running, publish it by selecting **Go Live** on the command bar.
1. Dynamics 365 Marketing copies the journey to its email marketing service, which executes the journey by processing contacts, performing actions, and collecting results during the time it is set to run. The journey's **Status Reason** is updated to Live.
1. It might take several minutes for your messages to get sent, so allow some time for them to arrive in your inbox. After they do, open them and load the images. Then you can go back to Dynamics 365 Marketing and see how your journey is going. The **Designer** tab now shows information and results for each tile from your pipeline. Open the **Insights** tab to see detailed analytics.


