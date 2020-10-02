---
lab:
    title: 'Lab 01: Explore Dynamics 365 Finance'
    module: 'Module 7: Introduction to Dynamics 365 Finance'
---

# MB-901: Dynamics 365 Fundamentals 
## Module 7, Lab 1 - Explore Dynamics 365 Finance 


**Prerequisites**: Prior to performing the steps of this lab, perform the
following tasks: 

**Note:** You need a deployed environment with demo data prior to perform
this lab. Your Dynamics 365 Finance and Operations apps instance can be
launched by directly going to the URL of the instance.

You will need to change the company to **USMF.** In order to login to the Dynamics 365 Finance and Operations apps instance you need to have a user name and password with either **Chief Executive Officer** or a **System administrator** security role.

In case your environment does not have demo data, follow the instructions
below:

Navigate to **Modules>Demo Data**, and click **Generate data** then click
    **OK.**

### Import exchange rates

1.  Change the company to **USMF.**

2.  Go to **General ledger > Currencies > Exchange rate types**.

3.  Click **New**.

4.  In the **Exchange rate type** field, type 'GTL-EXCH'.

5.  In the **Name** field, type 'Seahorse Exchange Rate'.

6.  Click **Exchange rates**.

7.  Note there is not any exchange rates available.

8.  Close Exchange rates form

9.  Close exchange rate type form

10. Go to **General ledger > Currencies > Configure exchange rate providers**.

11. Click **New**.

12. Select **Central Bank of the Russian Federation**

13. Click **OK**.

14. Close the page.

15. Go to **General ledger > Currencies > Import currency exchange rates**.

16. In the **Exchange rate type** field, enter or select GTL-EXCH

17. Select **Central Bank of the Russian Federation**

18. In the **Exchange rate provider** field, enter or select **Central Bank of
    the Russian Federation**

19. Click **OK**.

20. Go to **General ledger > Currencies > Exchange rate types**.

21. Select **GTL-EXCH**

22. Click **Exchange rates**.

23. Note the imported values

24. Close all forms

### Create a purchase order, post a product receipt

1.  Go to **Accounts Payables > Purchase orders > All purchase orders**.

2.  Click **New**.

3.  In the **Vendor account** field, select **1001 Acme Office Supplies**.

4.  In the **Warehouse** field, select **11**.

5.  Click **OK**.

6.  In the **Item number** field, Select item **1000 Surface Pro 128 GB**.

7.  On the Action Pane, click **Purchase**.

8.  Click **Confirm**.

9.  On the Action Pane, click **Receive**.

10. Click **Product receipt**.

11. In the **Product receipt** field, type **GTL02020**.

12. Click **OK**.

13. Close all forms.

### Create a free text invoice

1.  Go to **Accounts receivable > Invoices > All free text invoices**.

2.  Select **New**.

3.  In the **Customer account** field, select **US-003**.

4.  In the **Description** field, enter **Guide To Free Text Invoice**. in the
    dialog box click **Yes**.

5.  In the **Main account** field, select **110180** account number.

6.  In the **Quantity** field, enter **17**.

7.  In the **Unit price** field, enter **817.00**. The amount is calculated as
    the quantity times the unit price. However, you can override that
    calculation by entering an amount.

8.  Select **Charges** to add a charge to the invoice.

9.  In the **Charges code** field, enter **FREIGHT**.

10. In the **Charges value** field, enter **150**.

11. Close the page.

12. Select **Totals** to view a summary of the invoice details and totals.

13. Select **Close**.

14. Select **Post** to post the invoice. You will still have an opportunity to
    cancel before you actually post.

    -  You can change the timing of invoice printing. Select **Current** to
        print each invoice as it's updated. Select **After** to print after all
        invoices have been updated.

    -  To change how the customer's credit limit is verified before the invoice
        is posted, change the value in the **Credit limit type** field.

    -  To print the invoice, set the option to **Yes**.

    -  To post the invoice, set the option to **Yes**. You can print the
        invoice without posting it.

15. Select **OK**.
