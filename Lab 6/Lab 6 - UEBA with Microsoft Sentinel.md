# Lab 6 - UEBA with Microsoft Sentinel

## Exercise 1: Explore UEBA with Microsoft Sentinel

    ![program ](./media/image1.png)

You are a Security Operations Analyst working at a company that
implemented Microsoft Sentinel. Once you have connected your data
sources to Microsoft Sentinel, you can visualize and monitor the data
using the Microsoft Sentinel adoption of Azure Monitor Workbooks, which
provides versatility in creating custom dashboards.

Microsoft Sentinel allows you to create custom workbooks across your
data, and also comes with built-in workbook templates to allow you to
quickly gain insights across your data as soon as you connect a data
source.

### Task 1: Explore Entity Behavior

In this task, you will explore Entity behavior analytics in Microsoft
Sentinel.

1.  On the Azure
    Portal `http://portal.azure.com`,
    search for `Microsoft Sentinel` and
    click on **Microsoft Sentinel**.

    ![service ](./media/image2.png)

2.  Select **SwrkXXXXXXX**.

    ![](./media/image3.png)

3.  Now click on **Entity behavior** under Threat management.

    ![](./media/image4.png)

4.  On the popup from **Entity behavior settings**, select **Set UEBA**.

    ![](./media/image5.png)

5.  On the next page, you should notice that **UEBA** is already enabled
    as a part of the Deployment done in Lab 1.

    ![Screenshot](./media/image6.png)

    > **Note**: If UEBA is not On by default, turn it on from entity behavior
    settings.

    ![](./media/image7.png)

    ![](./media/image8.png)

6.  For the section **2. Sync Microsoft Sentinel with at least one of
    the following directory services**, notice the Microsoft Entra ID is
    already selected, click on the **Apply** button.

    ![](./media/image9.png)

    ![Screenshot](./media/image10.png)

7.  You should receive the Notification as shown in below image. The
    page will automatically be redirected to the Entity behaviour page.

    ![Screenshot](./media/image11.png)

8.  The confirms that the Entity behaviour is configured successfully.

    ![](./media/image12.png)

### Task 2: Confirm and review Anomalies rules

In this task, we will confirm if Anomalies analytics rules are enabled.

1.  While on the Microsoft Sentinel page click on **Analytics** under
    configuration, then select the **Anomalies** tab.

    ![](./media/image13.png)

2.  Select any rule and then select **Edit** on the rule blade.

    ![](./media/image14.png)

3.  Review the **General** tab information. Notice
    the **Mode** is **Production** and then select **Next:
    Configuration**.

    ![](./media/image15.png)

4.  Review the ***Configuration*** tab information. Notice that you
    cannot change the **Anomaly score threshold**.

    ![](./media/image16.png)

5.  Then select **X** in the top right corner to exit the Analytics rule
    wizard.

6.  Scroll right to the analytics rule you selected until see and select
    the ellipsis **(...)** icon. Select **Duplicate**

    ![](./media/image17.png)

7.  Scroll left to review the new rule with the **FLGT** tab at the
    beginning of the name. Select **FLGT** rule and then
    select **Edit** on the rule blade.

    ![](./media/image18.png)

8.  Review the **General** tab information. Set the status
    to **Enabled**, you will notice the **Mode** is **Flighting** and
    then select **Next: Configuration**.

    ![](./media/image19.png)

9.  Review the **Configuration** tab information. Notice that you can
    now change the **Anomaly score threshold**.

    ![video ](./media/image20.png)

10. Set the value to **1** and then select **Next: Submit Feedback**.

    ![](./media/image21.png)

11. Provide the feedback and then click on **Next: Review + create**.

    ![](./media/image22.png)

12. After the Validation is completed, click on Save button to update
    the rule

    ![](./media/image23.png)

    ![Screenshot](./media/image24.png)

13. If the **FLGT Analytic rule** still shows **Disabled**, then
    right-click on it and select **Enable** option.

    ![](./media/image25.png)

    ![Screenshot](./media/image26.png)

14. Now it should be enabled.

    ![](./media/image27.png)
