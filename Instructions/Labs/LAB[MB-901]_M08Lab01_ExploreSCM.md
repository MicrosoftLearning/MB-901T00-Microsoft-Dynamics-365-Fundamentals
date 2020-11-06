---
lab:
    title: 'Lab 01: Explore Dynamics 365 Supply Chain Management'
    module: 'Module 8: Introduction to Dynamics 365 Supply Chain Management'
---

# MB-901: Dynamics 365 Fundamentals 
## Module 8, Lab 1 - Explore Dynamics 365 Supply Chain Management

### Create a product

In **USMF**, you need to create a new item for a new configuration of cabinet to be purchased from vendors. 

1. Navigate to **Product information management** > **Products>Released products**.
1. Click **New**. 
1. In the **Product type** field, select **Item**
1. In the **Product subtype** field, select **Product**
1. In the **Product number** field, type **GTL007**
1. In the **Product name** field, type **Cabinet 2**
1. In the **Item model group** field, select **FIFO** (First In-First Out)
1. In the **Item group** field, select **TV&Video**
1. In the **Storage dimension group** field, select **SiteWH**
1. In the **Tracking dimension group** field, select **None**
1. In the **Inventory unit** field, select **ea** (Each)
1. In the **Purchase unit** field, select **ea** (Each)
1. In the **Sales unit** field, select **ea** (Each)
1. In the **BOM unit** field, select **ea** (Each)
1. In the **Purchase price** field, type **30.00**
1. In the **Sales price** field, type **30.00**
1. In the **Sales Taxation, Item sales tax group** field, select **ALL** (All sales tax codes)
1. In the **Purchase Taxation, Item sales tax group** field, select **ALL** (All sales tax codes)
1. Click **OK**.
1. Click **Validate** to ensure the product is completely finalized. This button is located on the product action pane.
1. Close all pages. 

### Create product masters

In **USMF**, you need to create a new item (V neck T-shirt) to buy.  This item will be available in size Small, Medium and Large and in colors: Black and Red.

1. Navigate to **Product information management** > **Products** > **Released products**.
1. Click **New**.
1. In the **Product type** field, select **Item**
1. In the **Product subtype** field, select **Product master**
1. In the **Product number** field, type **GTLPM001**
1. In the **Product name** field, type **V Neck T-Shirt**
1. In the **Search name** field, type **VNeckTShirt**
1. In the **Retail category** field, select **Apparel and Footwear**      
1. In the **Product dimension group** field, select **ColorSize**
1. In the **Configuration technology** field, select **Predefined variant**
1. In the **Item model group** field, select **FIFO** (First In-First Out)
1. In the **Item group** field, select **Audio** 
1. In the **Storage dimension group** field, select **SiteWH**
1. In the **Tracking dimension group** field, select **None**
1. In the **Inventory unit** field, select **ea** (Each)
1. In the **Purchase unit** field, select **ea** (Each)
1. In the **Sales unit** field, select **ea** (Each)
1. In the **BOM unit** field, select **ea** (Each)
1. In the **Sales Taxation, Item sales tax group** field, select **ALL** (All sales tax codes)
1. In the **Purchase Taxation, Item sales tax group** field, select **ALL **(All sales tax codes)
1. In the **Purchase price** field, type **19.95**
1. In the **Sales price** field, type **29.95**
1. Click **OK**. 
1. Close all pages.
1. Navigate to **Product information management** > **Products** > **Released products**.
1. Using quick filter search by item number for **GTLPM001**.
1. Click item **GTLPM001** to open the product master record.
1. Click the **Product dimensions** button from **Product action** pane.
1. Select the **Sizes** tab.
1. Click **New in the Define sizes for a product master** section.
1. In the **Size** field, enter **Small**.
1. In the **Name** field, enter **Small**.
1. In the **Description** field, enter **Small Size**.
1. Click **New**.
1. In the **Size** field, enter **Medium**.
1. In the **Name** field, enter **Medium**.
1. In the **Description** field, enter **Medium Size**.
1. Click **New**.
1. In the **Size** field, enter **Large**.
1. In the **Name** field, enter **Large**.
1. In the **Description** field, enter **Large Size**.
1. Select the **Colors** tab.
1. Click **New** in the **Define sizes for a product master** section.
1. In the **Color** field, enter **Black**.
1. In the **Name** field, enter **Black**.
1. In the **Description** field, enter **Black** color.
1. Click **New**.
1. In the **Name** field, enter **Red**.
1. In the **Description** field, enter **Red** color.
1. Click **Save**.
1. Close the form.
1. Click **Released Product variants** button from **Product action** pane.
1. Click **Variant suggestions** from **Product Variant action** pane.
1. Click **Select all**.
1. Click **Create**.
1. Close all pages.  

### Create a Purchase Order

Create one purchase order for Acme Office Supplies, to be delivered today, with 5 of item number T0003 to be delivered to Site 1, and 5 of M1101 Foam Reacting Agent to be delivered to the Quality Testing Center123 W. Cherry Street, Zip Code 83642.

1. Go to the **Procurement and sourcing** > **Purchase orders** > **All purchase orders**.
1. Click **New**.
1. **Vendor account:** Select **1001** (Acme Office Supplies)
1. **Delivery date:** Verify the current date in the **Delivery date** field (this should be the default value).
1. Click **OK**

### Add items to the purchase order

1. **Item number:** Select **T0003**.
1. **Quantity:** Enter **5**.
1. **Unit:** Enter **ea**.
1. Click **Add line**
1. **Item number:** Select **C0004**.
1. **Quantity:** Enter **4**.
1. **Unit:** Enter **pcs**.

### Select delivery addresses for the items

1. Select the line for item **T0003** in the **Purchase order lines** FastTab.
1. In the **Lines Details** fast tab, change to the **Address** tab.
1. Change the **Delivery address** to **Contoso Entertainment System USA**.
1. Select the line for item **C0004** in the **Purchase order lines** FastTab.
1. Change to the **Address** FastTab.  
1. Click the **Add address** button **(+)** to the right of the **Delivery address** field.
1. **Name or description:** Enter **Quality Testing Center**.
1. **Zip/postal code:** Enter **83642**.
1. **Street:** Enter **123 W. Cherry Street**.
1. Click **OK**.
1. Click **Save**.
1. On the **Action Pane**, click **Purchase**.  
1. Click **Confirm**.
1. On the **Action Pane**, click **Receive**.
1. Click **Product receipt**.
1. In the **Product receipt** field, enter the product receipt number. For example, enter **PR123**.
1. Click **OK** to post the product receipt.  
1. Close all pages.  

### Create sales orders

This procedure shows you how to create a sales order. You can use the procedure in demo data company USMF. Sales orders are typically created by a sales order processor.

1. Go to **Sales and marketing** > **Sales orders** > **All sales orders**.
1. Click **New**.
1. In the **Customer account** field, click the drop-down button to open the lookup.
1. In the list, find and select the customer **US-004**.
1. Click **OK**.
1. Click **Sales order line**.
1. Click **Dimensions**.
1. For this example, select the Color, Site and Warehouse dimensions. The dimensions you select here will appear in the sales order grid. If you want your selections to persist, set the **Save setup option** to **Yes**.
1. Click **OK**.
1. In the **Item number** field, click the drop-down button to open the lookup.
1. For this example, select item number **T0004**.
1. In the **Color** field, click the drop-down button to open the lookup.
1. In the list, find and select **Black**.
1. In the **Quantity** field, enter **1**.
1. On the **Action Pane**, click **Sales order**.
1. Click **Totals**.
1. The Totals page displays details about the entire order. This includes the subtotal amount, which is a sum of all line net amounts adjusted for eventual line discounts, the total invoice amount, which is a subtotal amount adjusted for eventual order-level discount, charges, and sales tax, the customer credit limit situation, and more. The invoice amount is the amount that will appear on the customer's invoice document.
1. Click **OK**.  
